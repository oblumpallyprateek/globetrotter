# Globetrotter — Decisions Log

## Milestone 0: Setup and Planning
- Destination chosen: Rio de Janeiro, Brazil
- Primary audience: First time travelers 
- One design decision that reflects the destination: Color-focused to show bold, vibrant that capture Rio's energy. I'll use the colors of the Brazillian flag (yellow, green, blue)
- Wireframe format used (hand-drawn / Figma / other): hand-drawn

## Milestone 1: HTML Structure

One HTML structure choice you made and why (e.g., why you used <article> instead of <div> for gallery items).

I used <article> elements for each attraction on the attractions page instead of just generic <div> tags because each attraction could stand alone on its own. 


One thing Claude generated that you changed, and why.

Claude generated that I should maybe include the top restraunts 
that everyone should try out in Rio. I changed this too include the top foods
they should try as I felt that was more important. 


One place where your wireframe guided a specific decision about structure.

My wireframe showed the home page with a hero section at the top, followed by an intro paragraph, then three preview cards right after. 

## Milestone 2: CSS Styling
One color or font choice you made, and why it serves your destination.

I chose Bebas Neue for headers because it's ultra-bold and designed for all-caps usage, which perfectly captures Rio's larger-than-life, energetic personality. The font feels like a festival poster and impossible to ignore, just like the city itself.


One Claude suggestion you rejected, and why.

Claude initially suggested Montserrat as the header font, but I rejected it in favor of Bebas Neue because I wanted maximum impact and energy.


One style that didn't look right at first, and what you changed.

When I first viewed the site, I noticed the food guide had the wrong content (gallery code was pasted in). The navigation links worked but took me to the wrong page. I replaced the gallery code with the correct food guide HTML, which fixed the issue and ensured each page displayed its intended content.


## Milestone 3: Flexbox Layout

One Flexbox property choice you made deliberately, and why.

I chose to use flex-wrap: wrap on the preview cards and gallery sections because it allows items to wrap to the next row naturally as the screen size changes. This creates a smoother transition between desktop (3 items per row) and mobile (1 item per row), and allows tablets to display 2 items side-by-side instead of forcing an all-or-nothing layou


One place where Claude generated a layout that didn't match your plan, and what you changed.

Claude's initial Flexbox implementation already matched my layout plan from planning.md. The navigation, preview cards, attractions, food entries, and gallery all used the correct Flexbox properties with proper spacing and mobile responsiveness. Since the generated CSS aligned with my wireframes and layout plan, I didn't need to change anything.


One layout challenge that required adjusting your HTML structure, and why.

The HTML structure already had proper container elements for Flexbox to work. For example, the preview cards needed a wrapper <div class="preview-cards"> around the three <article> elements so I could apply display: flex to the container. Without this wrapper, I couldn't control how the three cards arranged themselves horizontally. The container/item pattern (flex container wrapping flex items) is essential for Flexbox layouts to work properly.

## Milestone 4: Responsive Design
_Add entries after implementing media queries._

What breakpoints did you end up using, and why those values?

I used three breakpoints: Desktop (1024px+), Tablet (768px-1023px), and Mobile (767px and below). I chose 768px as the tablet breakpoint because that's the standard width for iPads and most tablets in portrait mode. The 1024px desktop breakpoint captures when there's enough screen space to comfortably display 3 cards side-by-side without them feeling cramped. These are industry-standard breakpoints that align with common device sizes.


One section where the mobile layout needed to feel genuinely different, and what you did.

The navigation bar needed to feel different on mobile, not just smaller. On desktop, the 4 links sit horizontally in a row, but on mobile I changed them to stack vertically with flex-direction: column. This makes the links much easier to tap with thumbs and gives each link more breathing room. The mobile navigation feels like a proper mobile menu rather than a squeezed desktop layout.


One Claude suggestion about breakpoints you accepted or rejected, and why.

I accepted Claude's suggestion to add a tablet breakpoint at 1023px for 2-column layouts on the preview cards and gallery. Initially, my CSS only had desktop (3 columns) and mobile (1 column), which meant tablets would show 3 cramped cards. The tablet breakpoint at 1023px creates a better intermediate experience where 2 cards per row look balanced and aren't too squeezed together.

## Stretch Features
_Add entries if you implement any stretch features._