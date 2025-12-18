# Learning IDP: Platform Engineering

This repository focuses on mastering Platform Engineering concepts and building Internal Development Platforms (IDP) using Backstage.io, service catalogs, and golden paths for developer self-service.

- [References](./REFERENCES.md)

## 🎯 Learning Objectives

By working through this repository, you will:

1. Understand Platform Engineering principles and philosophy
1. Master Backstage.io for building developer portals
1. Implement service catalogs and software templates
1. Design golden paths for common workflows
1. Build developer self-service capabilities
1. Integrate platform APIs and plugins
1. Measure platform adoption and developer experience

## 📚 Prerequisites

- Understanding of cloud infrastructure (Azure)
- Completed [learning-idp-infrastructure-as-code](https://github.com/vanHeemstraSystems/learning-idp-infrastructure-as-code)
- Completed [learning-idp-cicd-pipelines](https://github.com/vanHeemstraSystems/learning-idp-cicd-pipelines)
- Node.js 18+ and Yarn installed
- Docker and Kubernetes knowledge
- Git and GitHub account

## 🗂️ Directory Structure

```
learning-idp-platform-engineering/
├── README.md                          # This file
├── REFERENCES.md                      # Links to resources and related repos
├── .gitignore                         # Git ignore patterns
├── .env.example                       # Environment variables template
│
├── docs/
│   ├── concepts/
│   │   ├── 01-platform-engineering-overview.md
│   │   ├── 02-developer-experience.md
│   │   ├── 03-golden-paths.md
│   │   ├── 04-service-catalog.md
│   │   ├── 05-platform-apis.md
│   │   └── 06-platform-metrics.md
│   ├── guides/
│   │   ├── getting-started-backstage.md
│   │   ├── creating-templates.md
│   │   ├── plugin-development.md
│   │   ├── integrations.md
│   │   └── platform-adoption.md
│   └── examples/
│       ├── simple-service-catalog.md
│       ├── software-template.md
│       ├── custom-plugin.md
│       ├── platform-portal.md
│       └── golden-path-workflow.md
│
├── backstage/
│   ├── app/
│   │   ├── package.json
│   │   ├── tsconfig.json
│   │   └── src/
│   │       ├── App.tsx
│   │       ├── components/
│   │       └── theme/
│   │
│   ├── packages/
│   │   ├── backend/
│   │   │   ├── package.json
│   │   │   └── src/
│   │   │       ├── index.ts
│   │   │       └── plugins/
│   │   └── app/
│   │       ├── package.json
│   │       └── src/
│   │
│   ├── plugins/
│   │   ├── azure-devops/
│   │   │   ├── package.json
│   │   │   └── src/
│   │   ├── cost-insights/
│   │   │   ├── package.json
│   │   │   └── src/
│   │   └── platform-metrics/
│   │       ├── package.json
│   │       └── src/
│   │
│   ├── catalog/
│   │   ├── entities/
│   │   │   ├── components/
│   │   │   │   ├── api-service.yaml
│   │   │   │   ├── web-app.yaml
│   │   │   │   └── microservice.yaml
│   │   │   ├── systems/
│   │   │   │   ├── platform.yaml
│   │   │   │   └── product.yaml
│   │   │   ├── apis/
│   │   │   │   ├── rest-api.yaml
│   │   │   │   └── graphql-api.yaml
│   │   │   ├── resources/
│   │   │   │   ├── database.yaml
│   │   │   │   ├── storage.yaml
│   │   │   │   └── kubernetes.yaml
│   │   │   └── domains/
│   │   │       ├── platform.yaml
│   │   │       └── product.yaml
│   │   └── locations/
│   │       └── catalog-info.yaml
│   │
│   ├── templates/
│   │   ├── python-service/
│   │   │   ├── template.yaml
│   │   │   └── skeleton/
│   │   │       ├── catalog-info.yaml
│   │   │       ├── README.md
│   │   │       └── src/
│   │   ├── react-app/
│   │   │   ├── template.yaml
│   │   │   └── skeleton/
│   │   ├── azure-function/
│   │   │   ├── template.yaml
│   │   │   └── skeleton/
│   │   └── infrastructure/
│   │       ├── template.yaml
│   │       └── skeleton/
│   │
│   └── techdocs/
│       ├── default/
│       │   └── mkdocs.yml
│       └── components/
│
├── platform-apis/
│   ├── service-provisioning/
│   │   ├── src/
│   │   │   ├── main.py
│   │   │   ├── routers/
│   │   │   └── services/
│   │   └── tests/
│   │
│   ├── resource-management/
│   │   ├── src/
│   │   └── tests/
│   │
│   └── developer-portal/
│       ├── src/
│       └── tests/
│
├── golden-paths/
│   ├── web-application/
│   │   ├── README.md
│   │   ├── template.yaml
│   │   └── workflows/
│   │       ├── setup.yaml
│   │       ├── deploy.yaml
│   │       └── monitor.yaml
│   │
│   ├── api-service/
│   │   ├── README.md
│   │   ├── template.yaml
│   │   └── workflows/
│   │
│   ├── data-pipeline/
│   │   ├── README.md
│   │   ├── template.yaml
│   │   └── workflows/
│   │
│   └── infrastructure/
│       ├── README.md
│       ├── template.yaml
│       └── workflows/
│
├── examples/
│   ├── 01_basic_catalog/
│   │   ├── catalog-info.yaml
│   │   └── README.md
│   │
│   ├── 02_software_templates/
│   │   ├── python-service-template.yaml
│   │   ├── react-app-template.yaml
│   │   └── README.md
│   │
│   ├── 03_custom_plugins/
│   │   ├── cost-plugin/
│   │   ├── metrics-plugin/
│   │   └── README.md
│   │
│   ├── 04_techdocs/
│   │   ├── component-docs/
│   │   └── README.md
│   │
│   └── 05_integrations/
│       ├── azure-devops/
│       ├── github-actions/
│       └── README.md
│
├── automation/
│   ├── onboarding/
│   │   ├── create-project.py
│   │   ├── setup-permissions.py
│   │   └── configure-resources.py
│   │
│   ├── scaffolding/
│   │   ├── generate-service.py
│   │   └── generate-infrastructure.py
│   │
│   └── monitoring/
│       ├── track-adoption.py
│       └── measure-experience.py
│
├── metrics/
│   ├── dashboards/
│   │   ├── platform-adoption.json
│   │   ├── developer-experience.json
│   │   └── service-catalog.json
│   │
│   └── queries/
│       ├── usage-metrics.kql
│       └── experience-metrics.kql
│
├── infrastructure/
│   ├── backstage-deployment/
│   │   ├── kubernetes/
│   │   │   ├── deployment.yaml
│   │   │   ├── service.yaml
│   │   │   └── ingress.yaml
│   │   └── bicep/
│   │       └── backstage.bicep
│   │
│   └── platform-services/
│       ├── api-gateway/
│       └── service-mesh/
│
├── tests/
│   ├── unit/
│   │   ├── test_templates.py
│   │   └── test_plugins.py
│   │
│   ├── integration/
│   │   ├── test_catalog.py
│   │   └── test_workflows.py
│   │
│   └── e2e/
│       └── test_developer_flow.py
│
└── .github/
    └── workflows/
        ├── backstage-deploy.yml
        ├── template-validation.yml
        └── plugin-tests.yml
```

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/vanHeemstraSystems/learning-idp-platform-engineering.git
cd learning-idp-platform-engineering
```

### 2. Install Prerequisites

```bash
# Install Node.js 18+ and Yarn
# On Ubuntu/Debian:
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt-get install -y nodejs
npm install -g yarn

# Verify installations
node --version
yarn --version
```

### 3. Create Your First Backstage App

```bash
# Create Backstage app
npx @backstage/create-app@latest

# Navigate to app directory
cd my-backstage-app

# Start development server
yarn dev
```

### 4. Add Your First Service to Catalog

```yaml
# catalog-info.yaml
apiVersion: backstage.io/v1alpha1
kind: Component
metadata:
  name: my-first-service
  description: My first service in the platform
  annotations:
    github.com/project-slug: my-org/my-first-service
spec:
  type: service
  lifecycle: production
  owner: team-platform
  system: platform
```

## 📖 Learning Path

Follow this recommended sequence:

### Week 1: Platform Engineering Fundamentals

**Day 1-2: Platform Engineering Concepts**

1. Read `docs/concepts/01-platform-engineering-overview.md`
1. Study `docs/concepts/02-developer-experience.md`
1. Understand platform vs product thinking

**Day 3-4: Backstage.io Setup**

1. Follow `docs/guides/getting-started-backstage.md`
1. Set up local Backstage instance
1. Explore default plugins

**Day 5-7: Service Catalog**

1. Read `docs/concepts/04-service-catalog.md`
1. Add services to catalog
1. Define ownership and relationships

### Week 2: Software Templates & Golden Paths

**Day 1-3: Software Templates**

1. Study `docs/guides/creating-templates.md`
1. Work through `examples/02_software_templates/`
1. Create custom templates

**Day 4-7: Golden Paths**

1. Read `docs/concepts/03-golden-paths.md`
1. Design workflow golden paths
1. Implement in `golden-paths/`

### Week 3: Plugins & Integrations

**Day 1-4: Plugin Development**

1. Study `docs/guides/plugin-development.md`
1. Work through `examples/03_custom_plugins/`
1. Create custom plugin

**Day 5-7: Integrations**

1. Complete `docs/guides/integrations.md`
1. Integrate Azure DevOps
1. Configure GitHub Actions

### Week 4: Platform APIs & Metrics

**Day 1-3: Platform APIs**

1. Read `docs/concepts/05-platform-apis.md`
1. Build self-service APIs
1. Implement in `platform-apis/`

**Day 4-7: Metrics & Adoption**

1. Study `docs/concepts/06-platform-metrics.md`
1. Implement platform metrics
1. Track developer experience

## 🔑 Key Concepts

### Platform Engineering Principles

```
┌─────────────────────────────────────────┐
│     PLATFORM ENGINEERING GOALS          │
├─────────────────────────────────────────┤
│ 1. Reduce cognitive load               │
│ 2. Enable self-service                 │
│ 3. Standardize workflows               │
│ 4. Improve developer experience        │
│ 5. Increase development velocity       │
└─────────────────────────────────────────┘
```

### Golden Path Architecture

```
Developer Intent
      ↓
  Golden Path
      ↓
   Template
      ↓
  Automation
      ↓
   Resources
      ↓
  Monitoring
```

## 💡 Common Implementations

### Service Catalog Entry

```yaml
# catalog-info.yaml
apiVersion: backstage.io/v1alpha1
kind: Component
metadata:
  name: payment-service
  description: Payment processing microservice
  annotations:
    github.com/project-slug: my-org/payment-service
    azure-devops.com/project-repo: my-org/payment-service
  tags:
    - python
    - fastapi
    - payments
  links:
    - url: https://payment-api.example.com
      title: Production API
      icon: dashboard
    - url: https://docs.example.com/payment-service
      title: Documentation
      icon: docs
spec:
  type: service
  lifecycle: production
  owner: team-payments
  system: payment-platform
  dependsOn:
    - resource:payment-database
    - component:notification-service
  providesApis:
    - payment-api
```

### Software Template

```yaml
# templates/python-service/template.yaml
apiVersion: scaffolder.backstage.io/v1beta3
kind: Template
metadata:
  name: python-fastapi-service
  title: Python FastAPI Service
  description: Create a new Python FastAPI microservice
  tags:
    - python
    - fastapi
    - recommended
spec:
  owner: team-platform
  type: service
  
  parameters:
    - title: Service Information
      required:
        - name
        - description
        - owner
      properties:
        name:
          title: Service Name
          type: string
          description: Unique name for your service
          ui:autofocus: true
        description:
          title: Description
          type: string
          description: What does this service do?
        owner:
          title: Owner
          type: string
          description: Team owning this service
          ui:field: OwnerPicker
          ui:options:
            catalogFilter:
              kind: Group
    
    - title: Azure Configuration
      required:
        - resourceGroup
        - location
      properties:
        resourceGroup:
          title: Resource Group
          type: string
          description: Azure Resource Group name
        location:
          title: Location
          type: string
          description: Azure region
          enum:
            - westeurope
            - northeurope
            - eastus
          default: westeurope
  
  steps:
    - id: fetch-base
      name: Fetch Base Template
      action: fetch:template
      input:
        url: ./skeleton
        values:
          name: ${{ parameters.name }}
          description: ${{ parameters.description }}
          owner: ${{ parameters.owner }}
    
    - id: publish
      name: Publish to GitHub
      action: publish:github
      input:
        allowedHosts: ['github.com']
        description: ${{ parameters.description }}
        repoUrl: github.com?owner=my-org&repo=${{ parameters.name }}
    
    - id: register
      name: Register Component
      action: catalog:register
      input:
        repoContentsUrl: ${{ steps.publish.output.repoContentsUrl }}
        catalogInfoPath: '/catalog-info.yaml'
    
    - id: create-azure-resources
      name: Create Azure Resources
      action: azure:resource-group:create
      input:
        name: ${{ parameters.resourceGroup }}
        location: ${{ parameters.location }}
  
  output:
    links:
      - title: Repository
        url: ${{ steps.publish.output.remoteUrl }}
      - title: Open in Backstage
        icon: catalog
        entityRef: ${{ steps.register.output.entityRef }}
```

### Custom Plugin Structure

```typescript
// plugins/platform-metrics/src/plugin.ts
import { 
  createPlugin,
  createRoutableExtension,
} from '@backstage/core-plugin-api';

export const platformMetricsPlugin = createPlugin({
  id: 'platform-metrics',
  routes: {
    root: rootRouteRef,
  },
});

export const PlatformMetricsPage = platformMetricsPlugin.provide(
  createRoutableExtension({
    name: 'PlatformMetricsPage',
    component: () =>
      import('./components/PlatformMetricsPage').then(
        m => m.PlatformMetricsPage
      ),
    mountPoint: rootRouteRef,
  })
);
```

```typescript
// plugins/platform-metrics/src/components/PlatformMetricsPage.tsx
import React from 'react';
import { Grid, Card, CardContent, Typography } from '@material-ui/core';
import { InfoCard } from '@backstage/core-components';

export const PlatformMetricsPage = () => {
  const metrics = usePlatformMetrics();
  
  return (
    <Grid container spacing={3}>
      <Grid item xs={12} md={4}>
        <InfoCard title="Active Services">
          <Typography variant="h3">
            {metrics.activeServices}
          </Typography>
        </InfoCard>
      </Grid>
      
      <Grid item xs={12} md={4}>
        <InfoCard title="Deployments This Week">
          <Typography variant="h3">
            {metrics.weeklyDeployments}
          </Typography>
        </InfoCard>
      </Grid>
      
      <Grid item xs={12} md={4}>
        <InfoCard title="Developer Satisfaction">
          <Typography variant="h3">
            {metrics.satisfaction}%
          </Typography>
        </InfoCard>
      </Grid>
    </Grid>
  );
};
```

### Platform API Example

```python
# platform-apis/service-provisioning/src/main.py
from fastapi import FastAPI, HTTPException
from pydantic import BaseModel
from typing import List, Optional

app = FastAPI(
    title="Platform Service Provisioning API",
    description="Self-service API for provisioning platform services"
)

class ServiceRequest(BaseModel):
    name: str
    type: str
    owner: str
    environment: str
    config: dict

class ServiceResponse(BaseModel):
    id: str
    name: str
    status: str
    endpoints: List[str]
    repository_url: str

@app.post("/services", response_model=ServiceResponse)
async def create_service(request: ServiceRequest):
    """
    Create a new service using the platform's golden path
    """
    # Validate request
    if request.type not in ["api", "web", "worker"]:
        raise HTTPException(status_code=400, detail="Invalid service type")
    
    # Create from template
    service = await create_from_template(
        name=request.name,
        type=request.type,
        owner=request.owner
    )
    
    # Provision infrastructure
    infrastructure = await provision_infrastructure(
        service_id=service.id,
        environment=request.environment,
        config=request.config
    )
    
    # Register in service catalog
    await register_in_catalog(service)
    
    return ServiceResponse(
        id=service.id,
        name=service.name,
        status="provisioning",
        endpoints=infrastructure.endpoints,
        repository_url=service.repository_url
    )

@app.get("/services/{service_id}", response_model=ServiceResponse)
async def get_service(service_id: str):
    """
    Get service details
    """
    service = await fetch_service(service_id)
    if not service:
        raise HTTPException(status_code=404, detail="Service not found")
    return service
```

## 🎯 Best Practices

### 1. Design for Self-Service

```yaml
# Enable developers to provision their own resources
template:
  parameters:
    - user inputs (minimal)
  steps:
    - validate
    - provision
    - configure
    - register
    - notify
```

### 2. Implement Golden Paths

```
Golden Path = Template + Automation + Best Practices

Components:
- Pre-configured templates
- Automated workflows
- Built-in security
- Observability by default
- Documentation included
```

### 3. Measure Everything

```python
# Platform metrics to track
metrics = {
    "adoption": {
        "active_services": count,
        "template_usage": count,
        "developer_signups": count
    },
    "experience": {
        "time_to_first_deploy": duration,
        "template_completion_rate": percentage,
        "support_tickets": count
    },
    "performance": {
        "provisioning_time": duration,
        "deployment_frequency": rate,
        "success_rate": percentage
    }
}
```

### 4. Iterate Based on Feedback

```
Feedback Loop:
1. Gather developer feedback
2. Analyze pain points
3. Improve platform
4. Measure impact
5. Repeat
```

## 🔗 Related Repositories

- [learning-internal-development-platform](https://github.com/vanHeemstraSystems/learning-internal-development-platform) - Main overview
- [learning-idp-infrastructure-as-code](https://github.com/vanHeemstraSystems/learning-idp-infrastructure-as-code) - IaC for platform
- [learning-idp-cicd-pipelines](https://github.com/vanHeemstraSystems/learning-idp-cicd-pipelines) - Platform automation
- [learning-idp-api-development](https://github.com/vanHeemstraSystems/learning-idp-api-development) - Platform APIs
- [learning-idp-observability](https://github.com/vanHeemstraSystems/learning-idp-observability) - Platform monitoring

## 🤝 Contributing

This is a personal learning repository, but suggestions and improvements are welcome!

1. Fork the repository
1. Create a feature branch
1. Make your changes with tests
1. Ensure all tests pass
1. Submit a pull request

## 📄 License

This project is for educational purposes. See LICENSE file for details.

## 📧 Contact

Willem van Heemstra

- GitHub: [@vanHeemstraSystems](https://github.com/vanHeemstraSystems)
- LinkedIn: [Willem van Heemstra](https://www.linkedin.com/in/willemvanheemstra/)

-----

*Last updated: December 18, 2025*
*Part of the learning-internal-development-platform series*
