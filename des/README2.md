# Peter Millar Search Experience - UX Analysis

## Executive Summary
The Peter Millar search feature shows a disconnect between user intent and available actions. While the search overlay provides relevant product suggestions, users lack clear pathways to continue their search journey—no "View All" button, no way to re-search from the results page, and hidden filters that bury key shopping tools. These friction points likely contribute to the high abandonment rate, while those who do click through convert well because the Quick Shop feature is genuinely impressive.

*Note: Analysis conducted on 10/29/2025*

---

## Problem Identification

### Key Data Insights
- **High abandonment:** Users frequently leave Search without clicking products or viewing the Search Results Page
- **High conversion:** Users who click products from Search almost always purchase

### Primary Problems

#### Problem 1: No Clear Path to Search Results Page
**Description:**
The search overlay shows up to 6 product suggestions but provides no visual affordance to view all results. There's no "View All Results" button, "See More" link, or any indication that pressing Enter will take you to a full results page.

**Evidence:**
- Users must intuitively know to press Enter to reach the SRP—there's no UI element prompting this action
- Every other interactive element on the site (nav menus, account options) has explicit visual cues
- The Quick Shop overlay *does* include a "View Full Details" link, showing the pattern exists elsewhere
- "Your Recent Searches" feature doesn't actually work (or only works for logged-in users?), adding to confusion

**Impact:**
**This is likely the primary reason users abandon search.** Older users or those accustomed to clicking a search button may not realize they need to press Enter. Without a clear call-to-action, users hit a dead end and leave.

---

#### Problem 2: Filters Hidden Behind Extra Click
**Description:**
On the Search Results Page, all filters (category, size, fit, color) are collapsed by default. Users must click "Filter" to access these essential shopping tools.

**Evidence:**
- Filtering is one of the most common actions on e-commerce sites (see: Amazon, which always shows filters)
- The data shows users who reach products convert highly—but many abandon before getting there
- The "Filter" button is right-aligned, which goes against the left-to-right reading pattern

**Impact:**
"Out of sight, out of mind." If users don't immediately think to click the Filter button, they're stuck scrolling through unsorted results. This creates friction exactly when users need to narrow down options, likely contributing to abandonment.

---

#### Problem 3: Can't Re-Search from Search Results Page
**Description:**
Once on the SRP, there's no search input available. To perform a new search, users must click the search icon in the header again, which reopens the overlay.

**Evidence:**
- Users lose the ability to refine or change their search query mid-flow
- This breaks the search momentum—if initial results aren't quite right, users have to backtrack
- Most e-commerce sites maintain search functionality throughout the experience

**Impact:**
Users who realize their search query wasn't quite right face unnecessary friction to try again, increasing likelihood of abandonment.

---

## Additional UX Issues Worth Noting

### Search Overlay Polish
- **Visual inconsistency:** The live site shows a small fixed-width overlay, while screenshots show a full-width mega-menu style (which I actually think looked better). The small overlay makes product images tiny compared to the rest of the site's beautiful, large imagery.
- **Hover state inconsistency:** Nav menu links underline on hover, but search overlay links only turn blue. The titles also don't match the weight used in nav mega menus.
- **Interactivity gaps:** The Search button in the header doesn't turn navy on hover like other nav items. Also, it shifts position when toggling between "Search" and "Close" because it's not fixed-width.
- **Results clearing bug:** Clicking anywhere in the overlay that doesn't touch `#search-results` clears the results, which feels unintentional. Results should persist until the input changes or overlay closes.
- **Visual clutter:** You can hover over nav menu items while the search overlay is open, causing mega menus to appear behind it—creates visual clutter.
- **Page-specific bug:** On the Fit Philosophy page (https://www.petermillar.com/f/fit/fit-philosophy.html), some styles are affecting the search overlay.
- **Content in search:** The overlay can search page content, not just products. This feels like a distraction from getting users to shop.

### Search Results Page Polish
- **Missing tooltips:** "Tailored Fit" should have a tooltip explaining the tailoring process—couldn't find info on the SRP or product pages.
- **Quick Shop feedback:** In the Quick Shop overlay, the review stars show a pointer cursor but aren't clickable.
- **Scroll visibility:** The Quick Shop image carousel shows a subtle "Scroll" prompt, but it's easy to miss (opaque white with grey text). A scrollbar or using primary navy with white text would help.
- **Pre-footer CTA:** "Sign Up For Exclusives" feels generic—what exclusives do I actually get?

---

## Proposed Solutions

### Priority 1: Add "View All Results" to Search Overlay
**Current State:** No button or link to view full search results

**Proposed Change:** Add a "View All Results for '[query]'" link below the 6 suggested products, or add a prominent Search button next to the input field

**Rationale:** Gives users a clear, explicit action to take. Removes guesswork and accommodates users who don't think to press Enter.

**Expected Outcome:** Reduce search abandonment by providing an obvious next step. Should increase traffic to SRP significantly.

---

### Priority 2: Show Filters by Default on SRP
**Current State:** Filters collapsed behind "Filter" button (right-aligned)

**Proposed Change:** Display filters expanded by default on the left side of the page. Make it click-to-hide instead of click-to-show. If keeping a toggle, move the "Filter" button to the left.

**Rationale:** Filtering is a primary user need on results pages. Making it immediately visible reduces friction and helps users find products faster.

**Expected Outcome:** Users can narrow results immediately, increasing likelihood of finding and clicking products. Should improve click-through rate from SRP.

---

### Priority 3: Add Persistent Search Input to SRP
**Current State:** No way to search again without returning to header

**Proposed Change:** Include a search input field at the top of the SRP, either integrated into the page header or as a persistent element

**Rationale:** Lets users refine searches without breaking their flow. Reduces friction for users who need to adjust their query.

**Expected Outcome:** Keeps users in the search flow, reducing abandonment when initial results don't match intent.

---

## Conclusion
The Peter Millar search feature has a solid foundation—the Quick Shop feature is genuinely excellent, and the high conversion rate proves that users who reach products are ready to buy. The problem isn't the product selection or final experience; it's the gaps in the journey getting there. By adding explicit navigation (View All button), reducing filter friction, and maintaining search functionality throughout, we can bridge these gaps and convert more of those initial search intents into purchases.

The data tells us the destination is good—we just need to make the path clearer.