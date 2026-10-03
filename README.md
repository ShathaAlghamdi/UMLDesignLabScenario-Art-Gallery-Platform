# UMLDesignLabScenario-Art-Gallery-Platform

## Description

Art Gallery Platform is an online platform designed to connect artists with potential buyers.

The platform provides artists with a digital space to display and manage their artworks instead of relying only on physical galleries. Visitors can browse available artworks, view artwork details, purchase artworks, and make payments through the platform.

This project focuses on analyzing and modeling the system using UML before implementation.

## Problem

Traditional art galleries can limit the exposure of artists because artworks are displayed in physical locations and may only be seen by a limited number of visitors.

The Art Gallery Platform provides an online alternative where artists can showcase their artworks to a wider audience and visitors can discover and purchase artworks directly through the platform.

## Main Classes

The system contains the following main classes:

### User

Represents a general user of the platform.

Artist, Visitor, and Admin inherit from User.

Main attributes:
- user_id
- name
- email
- password

Main methods:
- login()
- logout()

### Artist

Represents an artist who publishes artworks on the platform.

Main attribute:
- bio

Main methods:
- uploadArtwork()
- updateArtwork()
- removeArtwork()

### Visitor

Represents a visitor or potential buyer.

Main methods:
- browseArtworks()
- viewArtwork()
- purchaseArtwork()

### Admin

Represents an administrator responsible for managing the platform.

Main methods:
- manageUsers()
- manageArtworks()

### Artwork

Represents an artwork displayed for sale.

Main attributes:
- artwork_id
- title
- description
- price
- image_url
- available

Main methods:
- viewDetails()
- updateAvailability()

### Payment

Represents a payment made when purchasing an artwork.

Main attributes:
- payment_id
- amount
- status

Main method:
- processPayment()

## Relationships

- Artist is a User.
- Visitor is a User.
- Admin is a User.
- An Artist can create multiple Artworks.
- A Visitor can purchase multiple Artworks.
- A Visitor can make multiple Payments.
- A Payment is associated with an Artwork.
- An Admin can manage Users.
- An Admin can manage Artworks.

## Main Use Cases

### Artist

- Upload artwork
- Update artwork
- Remove artwork
- Manage displayed artworks

### Visitor

- Browse artworks
- View artwork details
- Purchase artwork
- Make a payment

### Admin

- Manage users
- Manage artworks

## UML Modeling

The project uses UML diagrams to represent the structure and behavior of the Art Gallery Platform.

The class diagram includes:

- Classes
- Attributes
- Methods
- Inheritance
- Associations
- Multiplicities

## Tools

- UML
- Mermaid
- Git
- GitHub

## Authors

- Dana Ibrahim Alsalman
- Shatha Taha Alghamdi
- Lujain AbdulMohsen Alsultan
