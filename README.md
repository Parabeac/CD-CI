# A New DevOps Category - Continuous Design/Continuous Integration
Over the past several years, the Parabeac team has been exploring new technologies and processes for enhancing application development. This is not a casual exercise, we invested into building several internal experiments/tools that were primarily related to design and development. Through our own tool development activity along with that of others, we sense an impending inflection point in the history of app development. Agile processes and DevOps tools have already become mature contributors to the evolution of developer operations by improving development, testing, and maintenance. The goal of this document is to acknowledge those legacy processes and tools, analyze recent innovations, and introduce a brand new family of developer technologies that we coin Continuous Design/Continuous Integration (CD/CI).

# Legacy Processes & Tooling

Even those new to developer operations quickly become aware of standard practices and tools used across development teams of all sizes. Today, those standard tools are Agile process and associated DevOps tools. So how did we get here?

### Traditional App Development Process: Waterfall

An appropriate starting point is five decades ago, when the term Waterfall began to be used in association with software development. Waterfall app development was segmented by role, and projects moved through dev phases as in an assembly line. When a problem arose, the “production line” had to completely stop (losing time and money), and developers were forced to roll back and wait on the appropriate team to make the required fix and complete testing before resuming full production. It was, in some respects, an industrial age approach to an information age process.

### Introducing Agile

Almost immediately, developers pushed against the linear frustration of Waterfall and by the 1990’s there was a set of competing, more kinetic and flexible methodologies. By 2001 these approaches had a name and a manifesto, Agile. Among its many innovations, Agile introduced a philosophy in which cross-functional teams collaborate on project phases simultaneously and communicate effectively. When issues arise in a particular phase, the affected team resolves it quickly in defined collaborative work efforts. Agile contends that it is the constant introduction and resolution of issues in an intensely iterative process that builds value and quality into the output product The transition from Waterfall to Agile led developer operations from an incremental and linear segmentation to an integrated, adaptive process that fostered feedback and faster development cycles in a way that was, well, agile.

### The Rise of DevOps

DevOps became the term used for the tooling infrastructure for Agile methodology and it enhanced much of this new development process by automating & integrating operations. Its key contribution was making processes  _continuous._Legacy DevOps tools address different parts of the Agile development cycle. Popular categories include:

**Continuous Integration & Continuous Deployment**  - Tools that enable teams to regularly and quickly add changes and deploy projects in an effort to minimize the amount of time and lag between releases. (CircleCI, Jenkins, Bamboo, TravisCI, Azure DevOps Pipelines)

**Issue Management**  - The tools for supporting thorough and consistent progress as a project is designed, developed, tested, integrated, and deployed. (Trello, JetBrains Space, Jira, Azure DevOps Boards)

**Distributed Hosting**  - Tooling that keeps code and projects centralized and consistent to all members on a project, focusing on maintaining a single source of truth for developers. Examples are GitHub, GitLabs, and Bitbucket.

There are many other areas where tooling is being developed to expand DevOps capabilities. But perhaps the most exciting, and potentially most impactful, are the recent innovations around the design and build layer.

# Recent Innovations in Design and Build

Since Parabeac began out of a custom software development shop that had been supporting startups around the U.S., we experimented with many different tools that could impact application development, specifically ones that target the 'design to build' part of the process. We analyzed the following categories by using many of these new tools on real projects.

### Low-Code/No-Code

Low-Code/No-Code tools are designed to enable creators to build full-stack applications with little or no code. No-Code tends to hyper-specialize in a specific portion of development while Low-Code approaches from a full-stack view.

No-Code tools are often used by entrepreneurs to launch Minimum Viable Products (MVPs) and by small and mid-sized businesses to solve operational problems or support discrete marketing efforts. No-Code enthusiasts (sometimes called “devsumers”), may stitch together many No-Code tools in building applications. Examples of these tools are Bubble, Glideapps, Airtable, Zapier.

Low-Code tools are frequently used by enterprise companies in which IT teams are creating internal tools or simple external applications on behalf of general business operations. These tools include Mendix, Vantiq, Unqork, Retool, 8base, Canonic.dev, etc. While many of the low-code providers have very similar tooling, such as an UI editor & low-code 'IDE' for writing logic, they often specialize in specific verticals. For example, Vantiq specializes in low-code applications made to connect to IoT devices.

### Design-to-Code & Handoff Tools

Design-to-Code tools are code generation tools that interpret design files and generate code. These files can be architecture design, UI/UX design, schema design, and others. These tools include Parabeac-Core, Supernova, Visual Paradigm, DraftBit, etc.

Handoff tools like Zeplin, Avocode, Miro, Figma, etc. aid the interaction between system design & development. These tools help the developer understand the communications that the designer makes through the design files but, unlike design to code tools, handoff tools do not actually generate code. They do, however, allow for continuous communications during the entire project.

### Review: Low-Code/No-Code

Expectations vary on the long term impact of low-code/no-code. Many argue that low-code/no-code will replace the entire development process, ultimately obsoleting traditional developers. Others argue that these tools have only specific use cases within the process. Historically, no-code has automated and replaced only a small subset of development in the various areas in which it has been adopted. Wordpress is an example of automating the development of static, manually created HTML and CSS sites. However, despite the impact Wordpress has had on website development, it has had minimal impact on web app development because project needs are generally too complex to automate and it is too difficult to integrate the no-code/low-code output into the developer workflow.

### Review: Design-To-Code & Handoff Tooling

Handoff tools give the developer more context, but while the process is continuous, it lacks direct integration into the workflow. In theory, design-to-code tools have a direct integration between design and development, but these tools do not ensure that the process is  _continuous_. When a designer hands over a new generation of design requirements for an existing project, there is an immediate requirement for manual copying and pasting. This is a frustrating nuisance that can become costly and time consuming as the project matures. Two main trends contribute both to the growth of these tools but also to the complexity in creating solutions that meet truly market expectations.

**Digital Whiteboarding**  - The design process has moved from the physical whiteboard to the digital whiteboard through tools such as Figma, Miro, and AdobeXD. Since design is now established digitally, this should have presented a clear opportunity to automate code generation. Why then is there no popular digital tool that performs high quality Unified Modeling Language (UML) to code generation? Tools that have attempted to do so have consistently failed to provide the quality of code demanded by developers. Adobe, for example, invested into building its AdobeXD to Flutter converter only to see it deemed unusable by many across the Flutter developer community because of the poor output code quality. What accounts for the difficulty? The reason is  _context-driven design_.

**Context-Driven Design**  - Though the use of digital programs to design has increased, the standardization of  _how_  we communicate has fragmented. Agile's impact on removing unnecessary segmentation within development teams has led to the disparagement of 'software architects' and a disagreement on how to design architecture and utilize UML. Teams created their own unique flavors of UML or diagrams to describe their designed architecture depending on the context of the project. UML's lack of standardization and functionality around architecture definition lead to UML diagrams that are too often ambiguous and subjective. Context-driven design was meant to solve this by making things simpler for other humans to read but in doing so it added complexity in the way non-human tools can interpret design files.

Digital whiteboarding introduced platforms that communicate as well as provide APIs for interpretation, but the rise of context-driven design complicates these interpretations. So, can a process be created that combines the benefits of both design-to-code and handoff? Can this process be continuous and integrated? And would anyone pay for tools like that if they existed?

# Market Validation

Customers are already paying for existing design and development tools even with all their shortcomings. Venture capital is flowing toward these platforms due to enormous returns for investors, and there is robust enterprise acquisition and development within the space.

That the appetite is huge should be no wonder. The world runs on the apps which designers and developers build. Application development and deployment software was a $169B global market in 2020. In 2018 there were 23 million developers globally, and that number is growing. These developers undergird a massive worldwide app deployment. Over 35 million applications on Windows exist today. Over 2.6 million mobile apps are in the Google Play Store and another 2.1 Million apps on Apple’s AppStore. Web apps without a companion mobile app dwarfs these numbers.

**Venture Capital**  
Venture capital has noticed. In just the last year there was \$7.4 billion deployed amongst 416 VC deals in DevOps companies, over a \$1 billion increase from the year before. The largest deal activity was in the app building and testing sector with \$1.7 billion. A sampling of successful raises just since 2019 show the breadth of investor interest across all categories: No-Code: (Bubble \$6.3M, Glide Apps \$3.6M, AirTable \$185M); Low-Code (Vantiq \$27.8M, Unqork \$207M); Design to Code and Handoff (DraftBit \$1.15M, FramerX \$24M, Zeplin \$1.5M, Miro \$50M, Figma \$50M). No wonder VCs are enthusiastic. Newly public companies like Jfrog, Atlassian, Sumo Logic are happily accessing capital on the public markets having IPO’d in the billions of dollars.

**Enterprise Activity**  
Another marker of demand for design to development tools is the enterprise appetite for acquisition. UXPin, a tool that continuously integrates UI/UX Design & React.js development, was acquired by Xenon Partners, a Japanese PE Fund. Swagger, a developmental standard for API design to code was acquired by SmartBear and Microsoft purchased Github in 2018 for $7.5B.

If enterprises are not acquiring the capability externally there are starting to build it internally. Toyota recently announced internal tools they have built to help with development of Flutter for their new vehicles. One of those internal tools was an in-house design to Flutter converter. Airbnb invested in building a tool to generate Sketch elements from a React.js file. Its specific purpose was to reduce the time between the design and development phase.

# Continuous Design/Continuous Integration

With demonstrated market demand reinforced by white hot investor interest, this sector will continue to grow, the question is, in what fashion?. The interaction among the many tools already in the design & development space alongside the common trends of DevOps all point to a completely new emerging category which we call "Continuous Design/Continuous Integration" or "CD/CI". What will CD/CI look like?.

First, it is important that from the very beginning we are precise in our definition of CD/CI. The driving goal of CD/CI is to remove the duplicated work from design into development. To be genuinely  __CD/CI_,_  a tool must satisfy what we call the “Parabeac test”, namely does the platform meet at minimum these three requirements:

-   Generate code
-   Allow for continuous design updates
-   Directly integrate the design workflow into the development workflow

To be considered CD/CI a tool must capture the continuous design process seen in handoff tools, and leverage the direct integration in design-to-code tools, For example, in a UI/UX Continuous Design/Continuous Integration platform, code should be generated each time the designer creates new UI updates, and those changes should be merged automatically through the use of git. Every design file automatically generates a pull request.

This will be transformative. Writing the design into code is redundant work because the developer is simply transcribing into code his interpretation of what the designer has already created and often doing so imperfectly. Automating design to development is a clear and compelling opportunity for a major leap forward in development productivity.

How major? According to industry observers, creating the user interface typically takes up to 60% of development time. This easily represents the most attractive opportunity since  _Agile_  itself to redefine how apps are built. Not only is it an enormous cost component in building apps, but mistakes between designers & developers increase the cost of the development even after launch.

### The Challenges

This brings us back to the question we raised earlier regarding UML to code; if CD/CI is so compelling why hasn’t it already been introduced? It is because while automating the conversion and integrating design & development make obvious sense, there are plenty of challenges. Because CD/CI represents a higher standard than simple design to code conversion those challenges are even greater.

Once again, the problems center around context-driven design which we mentioned earlier. More human-like design input (good), makes interpretation complex (bad). CD/CI tools will support context-driven input, but they will also need context-driven output. To establish context-driven input, tools will need to create protocols or standards to which the input will map. To establish context-driven output, tools will need to ensure the way they generate code is both configurable and dynamic. Each development team has its own set of design patterns and its own standard for “quality code” so expecting a statically generated code converter to meet that broad set of very specific and different expectations is a bad bet. The tool must be manipulable and flexible in order to produce output code that will impress.

Many current tool providers have underestimated the critical requirement of high quality code and ignored the fact that each developer team programs in their own unique way. It takes substantial investment and repeated iteration to create a tool that generates code that is both high quality and highly configurable. Early providers have tried to be all things to all developers and have ended up being nothing for anyone. Consequently, the market for effective tools is likely to fragment around specific development frameworks because the best platforms will be ones that have selected sweet spots against which to direct their resources.

At Parabeac we approached those challenges with two specific strategies that may likely be adopted by future CD/CI providers in other segments of the category. First, to meet the output quality demands we chose to focus on one output format, and only one. We standardized on Flutter, precisely because we could direct all our resources to it and, in doing so, become the design-to Flutter experts and produce truly excellent output. We just could not accomplish that if we were trying to force one tool to generate in multiple output formats.

CD/CI platforms that specialize on a specific framework to increase code quality bring the potential to extend directly into the low-code/no-code space with capabilities much more attractive than the category’s current products. Existing low-code/no-code tools like Bubble do not produce actual code which means developers cannot create plugins for it; others like Wordpress generate code so complex that it is not usable. Because specialized CD/CI platforms will actually generate quality code, those technical limitations disappear.

Parabeac’s second major strategy to make certain we were building what developers actually needed and that our code was aligned to real-time developer demands is familiar but critical to CD/CI: open-source. A global open-source community means active developers constantly contributing to the way our generator exports code. The community becomes the real-time standard of excellence and utility for a CD/CI platform. By relying on an open-source strategy we do not decide what developers think is high quality; developers themselves do.

As CD/CI tools mature, they will reinvent bilateral communication between design & development. To continue the improvement of the CD/CI workflow, changes on the development side will need to be communicated back to the designer. The ideal functionality is one in which the tool automatically turns every design change into a pull request in git. In order to start that flywheel, Parabeac chose to create a design language to map design files to Sketch & Figma on the input side. We fully expect proliferation of the ‘CD/CI’ category will eventually include other design tools and platform choice and codegen extensibility.

### The Opportunity

The path forward is Continuous Design/Continuous Integration. CD/CI is not a replacement or a repudiation of Agile; in important ways it is Agile’s natural extension. Agile gave adaptive energy to the build and deploy stages of app development. CD/CI simply extends that backward to include the design stage as well. CD/CI, like Agile, integrates previously segmented workflows and embraces frequent iteration. In Agile’s case the process led to the development in recent decades of a fleet of new DevOps tools. CD/CI may mature in reverse; the true CD/CI tools that are just now appearing at Parabeac and elsewhere will lead the extension of process transformation in the design stage in ways that we, frankly, can only imagine. When CD/CI platforms become an integral part of automating developer workflows, the staggering 60% potential reduction in development costs may actually be a smaller long term benefit than the unshackled design creativity that can now be purely and seamlessly translated into code.
