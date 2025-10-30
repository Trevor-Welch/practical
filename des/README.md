# Peter Millar - Search Feature Analysis
The following contains feedback as the website was on 10/29/2025.

## Overview
Lorem ipsum dolar set

---

## Areas Of Improvements & Suggestions

#### AJAX Search Box
- The screenshots provided, and the live website are not the same. The screenshots show a large full-width mega-menu styled search box, which I actually think looks good. The live website, however, shows a small fixed width overlay card.
- The rest of the website has large beautiful images, but the search box is the smallest images a user will see. In the screenshot, the images easier to view as there is more screen real estate to work with.
- There is no "View All Results" CTA in the search overlay. **This may be the reason people aren't proceeding to the SRP.** While it makes sense to just press enter to start the search, some older users may be used to clicking a "search" button or a magnifying button to begin a search. There is no button to search and nothing that tells you to press enter. I believe just a simple "show all" link below the 6 results shown is all that is needed at minimum. 
- "Your Recent Searches" doesn't seem to actually store my recent searches. Is it a feature only for logged in users? If so, I'd like to hide it altogether.
- It seems that if I click anywhere within the search overlay that doesnt touch **#search-results** it clears the results. If I focus the input element, it re-loads the results. I'm not sure if this is intentional, but I feel like the results should stay shown until the input value changes or the overlay is closed.
- I'm not a big fan of how you are able to have the search overlay open, but still hover over the nav menu items to show the associated mega menu. Feels like visual clutter, but if the search results box was larger, it would at least hide this.
- I noticed a strange issue on https://www.petermillar.com/f/fit/fit-philosophy.html while clicking around. It looks like there are some styles on this page that are affecting the search overlay's styles.
- It seems that you can only search Content on the website using this search overlay. I almost don't even want to suggest page content. It feels like a distraction from getting the user to focus on shopping.

### Search Results Page (SRP)
- The filters being hidden by default feels like an extra click I have to make to do an action that is pretty common on an ecommerce website. Go to Amazon.com and search for something. They don't hide the filter because they know you're going to use it. A common UX quote I like to reference is something along the lines of "out of sight, out of mind". If a user doesn't immediately think to sort by category, size, fit, color, etc then they may not even think to filter to find what they are looking for. We should go ahead and make it click to hide, instead of click to show. If anything, the "Filter" button should be left aligned, since people look to the upper left first.
- I wish I could search on the SRP. If I want to perform a new search, I have to click the search button in the upper right again.
- I feel like there should be a tooltip that shows when you hover over "Tailored Fit". I couldn't find anything on the SRP or the Single Product page that explains how the tailoring process works.
- The "Quick Shop" feature is cool as heck, no wonder people who make it to the SRP end up buying something. The shopping experience is interesting. Going back to the Search Overlay missing a "view all" link, I noticed that the Quick Shop overlay **does** have a "View Full Details" link.
- In the Quick Shop overlay, the Reviews stars show a pointer when you hover, yet it is not interactable.
- It is a small touch that's probably not needed, but a scroll bar that shows while scrolling the product images in the Quick Shop overlay would be a nice, niche UX improvement. I didn't even notice the "Scroll" prompt that shows when you first open the Quick Shop overlay at first, even when disecting the UI like now. Maybe using the primary navy with white text instead of the opaque white with grey text?
- "Sign Up For Exclusives" as the pre-footer CTA feels... a bit dry. What kind of exclusives do I get?