# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static website for Faithful Friends Pet Care, a local pet sitting service in Transylvania County. The site is built with vanilla HTML, CSS, and JavaScript and deployed using Firebase Hosting.

## Development Commands

Since this is a static website, there are no build tools or package managers. Development is straightforward:

- **Local Development**: Open HTML files directly in a browser or use a local server
- **Deploy to Firebase**: `firebase deploy` (requires Firebase CLI and authentication)
- **Firebase Configuration**: Site is configured as "faithfulfriends" in firebase.json

## Site Architecture

### File Structure
- **Main Pages**: `index.html`, `about.html`, `services.html`, `contact.html`
- **Styles**: `styles.css` (main stylesheet), `themecolors.css` (color variables)
- **Images**: Logo and service images are hosted externally on WordPress
- **Firebase**: `firebase.json` configures hosting with `public/` as the deployment directory
- **Backup**: `backup/` directory contains previous versions of files

### Design System
The site uses a consistent design system defined in `styles.css`:

- **Colors**: Orange (`#ff8c42`) and amber (`#fbbf24`) primary palette
- **Typography**: Poppins for body text, Quicksand for headings
- **Components**: Reusable button, card, form, and navigation components
- **Responsive**: Mobile-first design with desktop breakpoints at 768px
- **Animations**: Hover effects, transitions, and subtle animations throughout

### Navigation Structure
All pages share the same navigation structure:
- Fixed header with logo and menu
- Mobile hamburger menu for smaller screens
- Consistent footer with contact information and social links

### Image Hosting
Images are externally hosted on WordPress (`faithfulfriendspetcare.wordpress.com`) and referenced via absolute URLs in the HTML.

## Firebase Hosting Configuration

The site is configured for Firebase Hosting with:
- Site name: "faithfulfriends" 
- Public directory: "public"
- Files are deployed from the `public/` directory, not the root

## Mobile Responsiveness

The site is fully responsive with:
- CSS Grid and Flexbox layouts
- Mobile-first CSS with desktop media queries
- Collapsible mobile navigation menu
- Touch-friendly button and link sizing