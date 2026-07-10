# 2026_InofrmationHealth

## UI design rules

- The theme picker has a neutral page surface, but every option card is always rendered in its own theme: Basic stays neutral, Media Quest stays navy/gold, and Wanko Challenge stays light blue/cream. Selecting one card must not recolor the other cards.
- Mobile must expose Theme as a labeled item in the Home bottom navigation and as a labeled action in Profile. Do not rely on an unlabeled gear icon or a Profile-only route for theme discovery.
- Each theme must keep readable foreground/background contrast across home, check, reaction, profile, and settings screens.
- Reaction choices use the shared line-icon system instead of emoji standing in for interface icons.
- Badge artwork is theme-specific: provided glossy rank images belong to Basic; Media Quest uses its own game emblems. The badge image is the avatar frame/background itself, with the person icon or account mark layered above it throughout the feed. The icon layer must be fully opaque and must not allow the badge artwork to show through its center. Rank badges must preserve a 1:1 aspect ratio at every size and theme; do not stretch them or add ribbon shapes that make the circular artwork look distorted. Image-backed badges must set background position, size, and repeat explicitly and be verified at both current-rank and badge-track sizes. A rank shown in Profile and the same rank used as a Home avatar frame must use the identical artwork, crop, scale, silhouette, and shadow; only the opaque account icon overlay may differ.
- The same screen must keep the same component hierarchy and visual language on desktop and mobile. Responsive rules may change available width, padding, and navigation placement, but must not substitute different headers, cards, badges, typography, or controls for the same content.
- Post cards should start with the avatar/account row and must not add category chips, “today's item” labels, or other tag-like metadata above it. Keep category and progress context in the surrounding challenge UI instead of duplicating it inside the post.
- Post action bars must stay on one line at every supported width. Show only the action icon and count visually; keep names such as Like, Comment, Repost, Save, and Share in accessible labels and tooltips.
