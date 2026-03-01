# Red Door Luxe: Revised Information Architecture

**Prepared for:** Dolli
**Prepared by:** Manus AI
**Date:** March 01, 2026

## 1.0. Executive Summary

The current Red Door Luxe demo site successfully showcases the *features* of the professional directory but buries the core value proposition — the **business solution for tenant retention and lead generation**. Key information regarding the service offering, pricing, and lead capture is located deep within a tabbed interface, requiring multiple clicks to access. This structure forces the user (the salon suite owner) to work too hard to understand the product.

This document outlines a revised information architecture designed to address this issue. The proposed strategy moves from a fragmented, tab-based layout to a **single, cohesive, long-form landing page**. This new structure will present a clear, linear narrative that guides the user from the market problem to our solution, with prominent calls-to-action for both the suite owner and prospective tenants.

## 2.0. Current Architecture: Audit & Analysis

The existing site is a single-page application divided into four main, hidden sections (tabs):

1.  **Welcome (`#page-welcome`):** Acts as a portal to the other three sections.
2.  **Our Professionals (`#page-directory`):** The core directory feature.
3.  **The Visibility Gap (`#page-gap`):** The market problem and opportunity.
4.  **Your Solution (`#page-solution`):** The product features, benefits, and primary call-to-action.

### 2.1. Identified Problems

| Buried Element | Current Location | Analysis |
| :--- | :--- | :--- |
| **Service Offering** | Buried in the "Your Solution" tab. | The full breakdown of what the directory includes is on the final tab, which a user may never navigate to. |
| **Pricing / Packages** | The "Offer Block" on the "Solution" tab has no price. | The core business offer is completely hidden. The user cannot evaluate the investment without scheduling a call, creating high friction. |
| **Lead Capture (Owner)** | The primary CTA ("Schedule a Call") is on the final "Solution" tab. | The main conversion goal is buried at the very end of the user journey. |
| **Lead Capture (Tenants)** | A "Lease a Suite" block is on the "Directory" tab. | This is a secondary goal and is logically placed, but its prominence could be improved. |

## 3.0. Proposed Strategy: A Unified Landing Page

The revised strategy is to eliminate the tabbed structure and rebuild the site as a **single, narrative-driven landing page**. This creates a logical flow that tells a story, guiding the user from problem to solution to conversion without requiring them to navigate.

The new page structure will be as follows:

1.  **Hero Section:** (Existing `welcome-hero`)
    *   **Headline:** Red Door _Luxe_ - A professional beauty directory...
    *   **Change:** Replace the two CTAs ("Meet Professionals" / "Why This Exists") with a single, primary CTA: **"See The Solution"** or **"View Packages"**. This immediately focuses the user on the business value.

2.  **The Problem: The Visibility Gap:** (Adapted from `#page-gap`)
    *   A concise, hard-hitting section that uses the key statistics (7,000+ searches, 83% use Google, etc.) to establish the market reality.

3.  **The ROI: The Cost of an Empty Suite:** (Adapted from `welcome-roi-strip`)
    *   Directly connect the market problem to the owner's bottom line. Frame the directory as a direct solution to tenant turnover.

4.  **The Solution: The Red Door Luxe Directory:** (New, consolidated section)
    *   **Headline:** "Your Digital Front Door."
    *   This section will prominently feature the **Packages / Pricing**.
    *   It will visually showcase the key features from the current "What's Included" list.

5.  **Lead Capture Block 1: For the Suite Owner**
    *   A clear, unmissable call-to-action to **"Schedule a 15-Minute Call"** or **"Choose a Package"**. This is the primary conversion point.

6.  **The Directory in Action: Professional Previews**
    *   Feature the existing professional cards (Gena, Tina, etc.) and the new "Prospective Professionals" as social proof and a live demonstration.

7.  **Lead Capture Block 2: For Prospective Tenants**
    *   The existing "Now Leasing" section, repurposed as a secondary CTA to attract new tenants to the building.

## 4.0. Next Steps

Upon approval of this strategy, the next phase will be to implement these architectural changes in the `index.html` file, transforming the site into the unified landing page outlined above. All existing content and styling will be repurposed within this new, more effective structure.
