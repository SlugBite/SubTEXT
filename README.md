# Subtext CMS
Subtext is not a blogging platform nor a static website builder; it is a modular content creation system.

The project is still in the planning phase.

Currently, database architecture and directory structure are nearly complete. Next is core development. Subtext utilizes a php framework. Yii2 is an option still, but CodeIgnitor is the likely choice. Lean and robust.

The biggest feature of Subtext is a content type generator accessible via the admin to quickly create new content types. Subtext makes no assumptions about what it will be used for beyond the default setup.

#### Out-Of-The-Box Functionality

- Taxonomies like categories, tags, and topics
- Default Entries content type for blogging or news
- Full SEO meta tag support
- Static hierarchical pages
- Hierarchical categories
- Pretty URLs by default
- Asset management for images, videos, and audio files
- Admin interface to create new content types that integrate with existing taxonomies or create new ones
- A themed system capable of quick interchangeability
- Comments system for entries and pages
- Social networking support for at least links and sharing
- Page view and share counting
- User management and authentication
- Role based permission system with ability to edit/create/remove built-in

Like-minded developers are welcome to join this project, particularly those experienced with AJAX and JavaScript.

#### Some Of The Guiding Principles

**Templating Engine** - Avoiding code-bloat is a top concern. If any templating language is used, it will be used sparingly. Constantly having to convert template tags into php is a bottleneck to be avoided. Particularly complex operations may use template tags to ease user modifications. Calling variables and functions will be the primary method of templating. In cases where template tags are used - if they end up being needed - Twig will likely be the language implemented.

**Use Only What You Want** - While a module or plugin system is planned for Subtext, the web has evolved to certain standards and they will be built into the platform with the ability to enable/disable each in the admin panel. Such features would include things like social sharing and lightboxes, among others.

**Create Content, Not Just Posts & Pages** - The fundamental inspiration behind Subtext is the ability to create *content*. Many CMSs merely allow you to create *certain types* of content and then pass off full content creation to third-party plugins, modules, components, or manual code modification. A perfect example of this is how WordPress uses Custom Post Types and Custom Fields.

An option-based admin panel for creating new content types with appropriate naming and detailed function selection is essential. While these new content types will be limited to structures used in default content types, combinations of all functionality will provide a greater degree of control. In advanced cases where information must be entered, processed, and/or displayed in a way that none of the default content types are, a module will step in to handle the task.

**Trees Are Forbidden** - The use of directory and document trees is expressly prohibited. Use of such a finite architecture imposes limits on the kind of sites that need a CMS most. We don't build 5-10 page sites for businesses anymore. Sites are ever-expanding dynamic libraries of content and they need a core document structure that allows for on-demand traversal of content, for both administrators and end-users.

**The M-V-C Approach** - I'm not a big fan of MVC. HMVC - or Layered MVC - is better but still presents the risk of bloating a system. Building the system on CodeIgnitor requires the use of Models, Views, and Controllers overall, though some deviation may occur where doing so will increase speed or efficiency.
