# References - Platform Engineering for IDP

This document contains curated resources for learning Platform Engineering and building Internal Development Platforms (IDP).

## 📚 Table of Contents

- [Official Documentation](#official-documentation)
- [Books](#books)
- [Articles & Blog Posts](#articles--blog-posts)
- [Video Tutorials](#video-tutorials)
- [Online Courses](#online-courses)
- [Tools & Libraries](#tools--libraries)
- [GitHub Repositories](#github-repositories)
- [Related Learning Repositories](#related-learning-repositories)
- [Community Resources](#community-resources)

-----

## 📖 Official Documentation

### Backstage.io

#### Core Documentation

- [Backstage Documentation](https://backstage.io/docs/overview/what-is-backstage) - Complete Backstage guide
- [Getting Started](https://backstage.io/docs/getting-started/) - Quick start guide
- [Architecture](https://backstage.io/docs/overview/architecture-overview) - System architecture
- [Tutorials](https://backstage.io/docs/tutorials/) - Step-by-step tutorials

#### Software Catalog

- [Software Catalog](https://backstage.io/docs/features/software-catalog/) - Catalog overview
- [Descriptor Format](https://backstage.io/docs/features/software-catalog/descriptor-format) - YAML format
- [System Model](https://backstage.io/docs/features/software-catalog/system-model) - Entity types
- [Well-known Annotations](https://backstage.io/docs/features/software-catalog/well-known-annotations) - Annotations

#### Software Templates

- [Software Templates](https://backstage.io/docs/features/software-templates/) - Template overview
- [Writing Templates](https://backstage.io/docs/features/software-templates/writing-templates) - Template creation
- [Built-in Actions](https://backstage.io/docs/features/software-templates/builtin-actions) - Template actions
- [Custom Actions](https://backstage.io/docs/features/software-templates/writing-custom-actions) - Custom actions

#### Plugins

- [Plugin Development](https://backstage.io/docs/plugins/) - Plugin overview
- [Backend Plugins](https://backstage.io/docs/plugins/backend-plugin) - Backend development
- [Frontend Plugins](https://backstage.io/docs/plugins/plugin-development) - Frontend development
- [Existing Plugins](https://backstage.io/docs/plugins/existing-plugins) - Available plugins

#### TechDocs

- [TechDocs](https://backstage.io/docs/features/techdocs/) - Documentation as code
- [Getting Started](https://backstage.io/docs/features/techdocs/getting-started) - Setup guide
- [Architecture](https://backstage.io/docs/features/techdocs/architecture) - TechDocs architecture

### Platform Engineering Concepts

- [Platform Engineering Overview](https://platformengineering.org/) - Platform engineering hub
- [CNCF Platforms White Paper](https://tag-app-delivery.cncf.io/whitepapers/platforms/) - CNCF guide
- [Team Topologies](https://teamtopologies.com/key-concepts) - Team structures
- [Internal Developer Platform](https://internaldeveloperplatform.org/) - IDP resources

-----

## 📚 Books

### Platform Engineering

1. **“Team Topologies”** by Matthew Skelton and Manuel Pais
- Team interaction patterns
- Platform team model
- [IT Revolution](https://itrevolution.com/product/team-topologies/)
1. **“Platform Engineering on Kubernetes”** by Maurício Salatino
- Building platforms on K8s
- Developer experience
- [Manning Publications](https://www.manning.com/books/platform-engineering-on-kubernetes)
1. **“Building an Internal Developer Platform”** by Luca Galante (Free eBook)
- IDP principles
- Implementation guide
- [Humanitec](https://humanitec.com/whitepapers/building-an-internal-developer-platform)

### Developer Experience

1. **“The DevOps Handbook”** by Gene Kim, Jez Humble, Patrick Debois, John Willis (2nd Edition)
- DevOps principles
- Platform thinking
- [IT Revolution](https://itrevolution.com/product/the-devops-handbook-second-edition/)
1. **“Accelerate”** by Nicole Forsgren PhD, Jez Humble, Gene Kim
- Measuring performance
- Key metrics
- [IT Revolution](https://itrevolution.com/product/accelerate/)

### Architecture

1. **“Building Evolutionary Architectures”** by Neal Ford, Rebecca Parsons, Patrick Kua (2nd Edition)
- Architecture patterns
- Change management
- [O’Reilly](https://www.oreilly.com/library/view/building-evolutionary-architectures/9781492097532/)
1. **“Software Architecture: The Hard Parts”** by Neal Ford, Mark Richards, Pramod Sadalage, Zhamak Dehghani
- Architecture decisions
- Trade-offs
- [O’Reilly](https://www.oreilly.com/library/view/software-architecture-the/9781492086888/)

-----

## 📝 Articles & Blog Posts

### Platform Engineering

#### Principles

- [What is Platform Engineering?](https://platformengineering.org/blog/what-is-platform-engineering) - Platform Engineering
- [Platform as a Product](https://martinfowler.com/articles/talk-about-platforms.html) - Martin Fowler
- [Building Internal Platforms](https://www.thoughtworks.com/insights/blog/engineering-excellence/building-internal-platforms) - ThoughtWorks

#### Implementation

- [How Spotify Built Their Platform](https://engineering.atspotify.com/2020/08/how-we-use-golden-paths-to-solve-fragmentation-in-our-software-ecosystem/) - Spotify Engineering
- [Netflix’s Platform Engineering](https://netflixtechblog.com/full-cycle-developers-at-netflix-a08c31f83249) - Netflix Tech Blog
- [Airbnb’s Service Platform](https://medium.com/airbnb-engineering/building-services-at-airbnb-part-1-c4c1d8fa811b) - Airbnb Engineering

### Backstage.io

#### Getting Started

- [Backstage Tutorial](https://backstage.io/blog/2020/03/16/backstage-tutorial) - Official blog
- [Adopting Backstage](https://backstage.io/blog/2021/07/20/adopting-backstage) - Adoption guide
- [Backstage Case Studies](https://backstage.io/blog/tags/case-study) - Real implementations

#### Advanced Topics

- [Custom Plugins](https://backstage.io/blog/2021/01/21/plugin-development) - Plugin development
- [Software Templates Deep Dive](https://backstage.io/blog/2021/07/26/software-templates-are-now-in-beta) - Templates guide
- [TechDocs Setup](https://backstage.io/blog/2020/09/08/announcing-tech-docs) - Documentation

### Golden Paths

- [Golden Paths at Spotify](https://engineering.atspotify.com/2020/08/how-we-use-golden-paths-to-solve-fragmentation-in-our-software-ecosystem/) - Spotify
- [Paved Roads at Netflix](https://www.youtube.com/watch?v=heoLFOhnYdw) - Netflix approach
- [Well-Lit Path](https://charity.wtf/2020/07/30/well-lit-path-vs-paved-road/) - Charity Majors

-----

## 🎥 Video Tutorials

### Platform Engineering

#### Conferences

- [PlatformCon 2023](https://platformcon.com/) - Platform engineering conference
- [What is Platform Engineering?](https://www.youtube.com/watch?v=ghzsBm8vOms) - Intro (20 min)
- [Platform as a Product](https://www.youtube.com/watch?v=lSd_4JMFXZs) - KubeCon (40 min)

#### Case Studies

- [Spotify’s Platform Journey](https://www.youtube.com/watch?v=vBnqJ5MbVZs) - QCon (45 min)
- [Netflix Full Cycle Developers](https://www.youtube.com/watch?v=0egFYt0VK-k) - Netflix (30 min)
- [Airbnb’s Service Platform](https://www.youtube.com/watch?v=xQGHWMw3X7w) - Airbnb (35 min)

### Backstage.io

#### Getting Started

- [Backstage Introduction](https://www.youtube.com/watch?v=85TQEpNCaU0) - Spotify (30 min)
- [Backstage Demo](https://www.youtube.com/watch?v=1XtJ5FAOjPk) - Live demo (45 min)
- [Building with Backstage](https://www.youtube.com/watch?v=PCWLxJ15rCw) - Workshop (2 hours)

#### Advanced Topics

- [Backstage Plugins](https://www.youtube.com/watch?v=qNe8OAirQY4) - Plugin dev (40 min)
- [Software Templates](https://www.youtube.com/watch?v=qYq4x3n8SzY) - Templates (35 min)
- [TechDocs in Action](https://www.youtube.com/watch?v=mOLCgdPw1iA) - Documentation (25 min)

-----

## 🎓 Online Courses

### Platform Engineering

#### Free Courses

- [Platform Engineering 101](https://www.youtube.com/playlist?list=PLzFsezKGlH4D2R0LKF3sR0J4UQZOw-Zb2) - YouTube series
- [Building Developer Platforms](https://www.infoq.com/presentations/platform-engineering/) - InfoQ
- [CNCF Webinars](https://www.cncf.io/online-programs/cncf-on-demand-webinar-platform-engineering-101/) - CNCF

### Backstage.io

#### Official Training

- [Backstage Learning Path](https://backstage.io/docs/getting-started/) - Official tutorials
- [Backstage Workshops](https://github.com/backstage/community/tree/main/workshops) - Community workshops

#### Video Tutorials

- [Complete Backstage Course](https://www.youtube.com/watch?v=4H_6CM9BSMA) - Full tutorial (3 hours)
- [Backstage for Beginners](https://www.youtube.com/playlist?list=PLVojzGZ4K8b) - Tutorial series

### Paid Platforms

#### Udemy

- [Platform Engineering Fundamentals](https://www.udemy.com/topic/platform-engineering/) - Course catalog
- [Backstage IDP Development](https://www.udemy.com/course/backstage-idp/) - Comprehensive

-----

## 🛠️ Tools & Libraries

### Backstage Ecosystem

#### Core

- **[Backstage](https://github.com/backstage/backstage)** - Platform framework
- **[@backstage/cli](https://www.npmjs.com/package/@backstage/cli)** - CLI tool
- **[@backstage/create-app](https://www.npmjs.com/package/@backstage/create-app)** - App generator

#### Popular Plugins

- **[@backstage/plugin-kubernetes](https://github.com/backstage/backstage/tree/master/plugins/kubernetes)** - Kubernetes integration
- **[@backstage/plugin-github-actions](https://github.com/backstage/backstage/tree/master/plugins/github-actions)** - GitHub Actions
- **[@backstage/plugin-azure-devops](https://github.com/backstage/community-plugins/tree/main/workspaces/azure-devops)** - Azure DevOps
- **[@backstage/plugin-cost-insights](https://github.com/backstage/backstage/tree/master/plugins/cost-insights)** - Cost tracking

### Platform Tools

#### Service Mesh

- **[Istio](https://istio.io/)** - Service mesh
- **[Linkerd](https://linkerd.io/)** - Lightweight service mesh
- **[Consul](https://www.consul.io/)** - Service networking

#### API Gateway

- **[Kong](https://konghq.com/)** - API gateway
- **[Azure API Management](https://azure.microsoft.com/en-us/products/api-management)** - Azure API gateway
- **[Ambassador](https://www.getambassador.io/)** - Kubernetes gateway

#### Developer Portals

- **[Backstage](https://backstage.io/)** - IDP framework
- **[Port](https://www.getport.io/)** - Developer portal
- **[Cortex](https://www.cortex.io/)** - Service catalog

### Infrastructure Tools

- **[Crossplane](https://www.crossplane.io/)** - Infrastructure provisioning
- **[ArgoCD](https://argo-cd.readthedocs.io/)** - GitOps for Kubernetes
- **[Flux](https://fluxcd.io/)** - GitOps toolkit
- **[Pulumi](https://www.pulumi.com/)** - Infrastructure as code

### Observability

- **[Prometheus](https://prometheus.io/)** - Metrics
- **[Grafana](https://grafana.com/)** - Visualization
- **[OpenTelemetry](https://opentelemetry.io/)** - Observability framework
- **[Jaeger](https://www.jaegertracing.io/)** - Distributed tracing

-----

## 💻 GitHub Repositories

### Official Repositories

#### Backstage

- [Backstage](https://github.com/backstage/backstage) - Main repository
- [Community Plugins](https://github.com/backstage/community-plugins) - Community plugins
- [Backstage Demo](https://github.com/backstage/demo) - Demo instance
- [Backstage Workshops](https://github.com/backstage/community/tree/main/workshops) - Workshop materials

### Example Implementations

- [RoadieHQ Examples](https://github.com/RoadieHQ/roadie-backstage-plugins) - Plugin examples
- [Backstage AWS](https://github.com/awslabs/aws-backstage-plugins) - AWS plugins
- [Backstage Azure](https://github.com/Azure/azure-backstage-plugins) - Azure plugins

### Platform Engineering

- [Platform Engineering Resources](https://github.com/Platformengineering/platform-engineering-resources) - Curated list
- [Awesome Platform Engineering](https://github.com/shospodarets/awesome-platform-engineering) - Resources
- [IDP Blueprints](https://github.com/cloud-platform-reference-architecture/platform) - Reference architecture

### Golden Path Templates

- [Backstage Templates](https://github.com/backstage/software-templates) - Official templates
- [Community Templates](https://github.com/topics/backstage-template) - Community templates
- [Enterprise Templates](https://github.com/RoadieHQ/software-templates) - Enterprise examples

-----

## 🔗 Related Learning Repositories

### From learning-internal-development-platform Series

1. **[learning-internal-development-platform](https://github.com/vanHeemstraSystems/learning-internal-development-platform)**
- Main overview
- Complete roadmap
1. **[learning-idp-infrastructure-as-code](https://github.com/vanHeemstraSystems/learning-idp-infrastructure-as-code)**
- Platform infrastructure
- IaC patterns
1. **[learning-idp-cicd-pipelines](https://github.com/vanHeemstraSystems/learning-idp-cicd-pipelines)**
- Platform automation
- Deployment pipelines
1. **[learning-idp-api-development](https://github.com/vanHeemstraSystems/learning-idp-api-development)**
- Platform APIs
- Service development
1. **[learning-idp-observability](https://github.com/vanHeemstraSystems/learning-idp-observability)**
- Platform monitoring
- Developer metrics
1. **[learning-idp-azure-security](https://github.com/vanHeemstraSystems/learning-idp-azure-security)**
- Platform security
- Access control

-----

## 👥 Community Resources

### Forums & Discussion

#### Official Communities

- [Backstage Discord](https://discord.gg/backstage-687207715902193673) - Main community
- [CNCF Slack #platformengineering](https://cloud-native.slack.com/) - CNCF channel
- [Platform Engineering Slack](https://platformengineering.org/slack) - Platform community

#### Discussion Boards

- [Backstage Community](https://github.com/backstage/community) - GitHub discussions
- [Platform Engineering Community](https://community.platformengineering.org/) - Forums

### Social Media

#### LinkedIn

- [Platform Engineering Community](https://www.linkedin.com/groups/13937144/) - LinkedIn group
- [#platformengineering](https://www.linkedin.com/feed/hashtag/platformengineering/) - Hashtag

#### Twitter/X

- [@BackstageIO](https://twitter.com/BackstageIO) - Official account
- [#platformengineering](https://twitter.com/hashtag/platformengineering) - Hashtag
- [#backstage](https://twitter.com/hashtag/backstage) - Hashtag

#### Reddit

- [r/platformengineering](https://www.reddit.com/r/platformengineering/) - Subreddit
- [r/devops](https://www.reddit.com/r/devops/) - DevOps discussions

### Blogs & Newsletters

- [Backstage Blog](https://backstage.io/blog/) - Official blog
- [Platform Engineering Newsletter](https://platformengineering.org/newsletter) - Weekly updates
- [Platform Weekly](https://platformweekly.com/) - Curated news
- [Internal Developer Platform Newsletter](https://internaldeveloperplatform.org/newsletter/) - IDP news

### Conferences & Events

- [PlatformCon](https://platformcon.com/) - Annual conference
- [BackstageCon](https://events.linuxfoundation.org/backstagecon-north-america/) - Backstage conference
- [KubeCon](https://www.cncf.io/kubecon-cloudnativecon-events/) - Cloud native
- [DevOps Enterprise Summit](https://events.itrevolution.com/) - Enterprise DevOps

-----

## 📊 Platform Metrics & KPIs

### Developer Experience Metrics

```
Lead Time for Changes
Deployment Frequency
Mean Time to Recovery (MTTR)
Change Failure Rate

Platform-Specific:
- Time to First Deploy
- Template Adoption Rate
- Developer Satisfaction Score
- Service Provisioning Time
```

### Platform Health Metrics

```
System Availability
API Response Times
Error Rates
Resource Utilization

Platform-Specific:
- Catalog Coverage
- Documentation Completeness
- Plugin Usage
- Support Ticket Volume
```

-----

## 📚 Essential Reading

### Core Papers

- [CNCF Platforms Definition](https://tag-app-delivery.cncf.io/whitepapers/platforms/) - CNCF white paper
- [Team Topologies for Platform Teams](https://teamtopologies.com/key-concepts-content/what-is-a-platform-team-in-team-topologies) - Team structure
- [Platform Engineering Maturity Model](https://platformengineering.org/platform-maturity-model) - Maturity assessment

### Case Studies

- [Spotify Platform Model](https://engineering.atspotify.com/2020/08/how-we-use-golden-paths-to-solve-fragmentation-in-our-software-ecosystem/) - Golden paths
- [Netflix Full Cycle Developers](https://netflixtechblog.com/full-cycle-developers-at-netflix-a08c31f83249) - Full cycle approach
- [Airbnb Service Platform](https://medium.com/airbnb-engineering/building-services-at-airbnb-part-1-c4c1d8fa811b) - Platform journey

-----

## 🎯 Next Steps

After mastering Platform Engineering, you can:

1. **Deploy production platform** - Launch your IDP
1. **Measure adoption** - Track platform metrics
1. **Iterate based on feedback** - Continuous improvement
1. **Share learnings** - Contribute to community

Additional learning:

- **[learning-idp-cicd-pipelines](https://github.com/vanHeemstraSystems/learning-idp-cicd-pipelines)** - Complete the IDP automation
- Join platform engineering communities
- Attend PlatformCon or BackstageCon
- Contribute to Backstage ecosystem

-----

*Last updated: December 18, 2025*
*Part of the learning-internal-development-platform series*
