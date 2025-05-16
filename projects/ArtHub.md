---
layout: project
type: project
image: img/landingpage_final (1).png
title: "ArtHub"
date: 2025
published: true
labels:
  - Database
  - Web Application
  - Next.js
  - Bootstrap-React
  - PostgreSQL

summary: "An online web application created as part of my ICS 314 group project."
---

ArtHub was an idea that came about after realizing there aren't many online applications that make it easy for artists to showcase their work. 
The application is not only supposed to help artists get eyes on their pieces but also provide a secure portal for art transactions. A user would first
sign up and then be able to create a profile. Through this profile, a user could showcase their 'Gallery', a sort of inventory of created/uploaded artworks.



[Github pages](https://arthub-final-project.github.io/arthub.github.io/)

[Vercel Deployment](https://vercel.com/jays-projects-2f307c71/arthub-314)
(if link does not work [click here](https://arthub-314-cyan.vercel.app/))



Personal duties on this project included:
- Creating the main landing page of the site.
  
- Creating database models for user gallery items.
  
- Creating a 'Gallery card' for a dynamic, real-time database view of a user's gallery item.
  
- Implementing 'Gallery card' functionality into the main landing page for a weekly artist showcase
  feature.

- Dealing with various issues as they came up, mostly relating to database retrieval bugs



## Source code for Gallery Card: 
```
    /* eslint-disable @next/next/no-img-element */

'use client';

import { Card } from 'react-bootstrap';
import { GalleryItem, User } from '@/lib/validationSchemas';

const GalleryCard = ({ user, gallery }: { user: User, gallery: GalleryItem }) => (
  <Card className="h-100 shadow-sm">
    <Card.Img
      variant="top"
      src={gallery.image}
      alt={gallery.title}
      style={{ height: '250px', objectFit: 'cover' }}
    />
    <Card.Body>
      <Card.Title>{gallery.title}</Card.Title>
    </Card.Body>
    <Card.Footer className="d-flex align-items-center gap-2">
      <img
        src={user.profileImage}
        alt={user.name}
        width={32}
        height={32}
        style={{ borderRadius: '50%' }}
      />
      <small className="text-muted">{user.email}</small>
    </Card.Footer>
  </Card>
);

export default GalleryCard;

```
