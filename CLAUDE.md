# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the corporate website for Verdafly (合同会社緑蝶 / Midoricho LLC), a digital entertainment content development company. The site is a single-page HTML application hosted on GitHub Pages with a custom domain (www.verdafly.com).

## Architecture

**Static Website Structure:**
- Single-page application built with vanilla HTML, CSS, and JavaScript
- No build process or package manager required
- Hosted on GitHub Pages
- Uses CDN-hosted dependencies (Tailwind CSS, Font Awesome, Google Fonts)

**Key Technologies:**
- Tailwind CSS 2.2.19 for styling
- Font Awesome 6.4.0 for icons
- Noto Sans JP font for Japanese typography
- Vanilla JavaScript for interactivity (mobile menu, smooth scrolling)

**Content Sections:**
- Hero section with company branding
- Company overview (会社概要)
- Services (事業内容) - Digital games, text content, sound content, mobile apps, solutions
- Clients (主要取引先) - Amazon, DLsite, DMM
- Company information (会社情報) - Legal details and registration
- Contact form (お問い合わせ)

## Development

**Viewing the Site:**
- Open `index.html` directly in a browser
- No local server required for basic development

**Deployment:**
- Push changes to the `main` branch
- GitHub Pages automatically deploys from the main branch
- Custom domain configured via `CNAME` file

## Design System

**Brand Colors:**
- Primary green: `#228B22` (verdafly-green)
- Accent green: `#4CAF50` (used in butterfly icon)
- Background green: `rgba(76, 175, 80, 0.05)` (butterfly-bg)

**Custom Components:**
- `.butterfly-icon`: Custom CSS-based butterfly logo (no image files)
- `.butterfly-wing`, `.butterfly-body`: SVG-like shapes using pure CSS
- `.header-link`: Animated underline effect on hover

**Responsive Design:**
- Mobile-first approach
- Breakpoints using Tailwind's `md:` prefix
- Mobile menu toggle for small screens
- Fixed header with shadow

## Content Structure

The site is fully bilingual (Japanese primary) with the following business information:
- Company: 合同会社緑蝶 (Midoricho LLC)
- Brand: Verdafly (ヴァダフライ)
- Established: January 31, 2025
- Location: Tokorozawa, Saitama Prefecture
- Business: Digital entertainment content development

## JavaScript Functionality

**Mobile Menu:**
- Toggle visibility with hamburger button
- Auto-close when clicking menu items

**Smooth Scrolling:**
- Anchor links scroll to sections with offset for fixed header
- Header offset: 80px

## Important Notes

- The contact form (index.html:379-399) is currently non-functional (no backend)
- All content is hardcoded in HTML (no CMS or data layer)
- No JavaScript framework dependencies
- The site is optimized for Japanese audiences
