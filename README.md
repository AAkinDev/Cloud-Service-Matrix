# Cloud Service Matrix ☁️

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](CONTRIBUTING.md)
[![Last Updated](https://img.shields.io/badge/last%20updated-2025--08--03-blue.svg)](https://github.com/AAkinDev/Cloud-Service-Matrix)

A comprehensive comparison matrix of cloud services across major providers, including **AWS**, **Azure**, **Google Cloud Platform**, **Oracle Cloud**, and **IBM Cloud**.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Quick Start](#quick-start)
- [Data Structure](#data-structure)
- [Usage Examples](#usage-examples)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This repository provides a detailed comparison of cloud services, helping developers, architects, and decision-makers make informed choices when selecting cloud providers and services for their projects. Whether you're building a new application, migrating existing infrastructure, or evaluating cloud options, this matrix serves as your comprehensive reference guide.

### Cloud Providers Overview & Market Share (2025)

| Rank | Provider | Logo | Market Share | Coverage | Position |
|------|----------|------|-------------|----------|----------|
| **🥇 #1** | **Amazon AWS** | ![AWS Logo](https://raw.githubusercontent.com/AAkinDev/Cloud-Service-Matrix/main/assets/logos/aws.png) | ~31% | 100% | **🏆 Market Leader** |
| **🥈 #2** | **Microsoft Azure** | ![Azure Logo](https://raw.githubusercontent.com/AAkinDev/Cloud-Service-Matrix/main/assets/logos/Azure.png) | ~25% | 100% | **🥈 Enterprise Focus** |
| **🥉 #3** | **Google Cloud** | ![Google Cloud Logo](https://raw.githubusercontent.com/AAkinDev/Cloud-Service-Matrix/main/assets/logos/Google_cloud.png) | ~11% | 100% | **🥉 AI/ML Leader** |
| #4 | **Oracle Cloud** | ![Oracle Cloud Logo](https://raw.githubusercontent.com/AAkinDev/Cloud-Service-Matrix/main/assets/logos/oracle-cloud.png) | ~3% | 100% | Database Specialist |
| #5 | **IBM Cloud** | ![IBM Cloud Logo](https://raw.githubusercontent.com/AAkinDev/Cloud-Service-Matrix/main/assets/logos/IBM_Cloud_logo.png) | ~2% | 100% | Enterprise Solutions |
| #6+ | **Others** | - | ~28% | Limited | (Alibaba Cloud, DigitalOcean, Linode, Vultr, Heroku, Salesforce, SAP, VMware, Rackspace, OVHcloud) |

## ✨ Features

- **📊 Comprehensive Coverage**: 16+ service categories across 5 major providers
- **🔄 Multiple Formats**: CSV for analysis, Markdown for documentation, Notion for collaboration
- **📈 Regular Updates**: Maintained with latest service information
- **🎨 Visual Organization**: Categorized by service type for easy navigation
- **🔗 Notion Integration**: Ready-to-use template for team collaboration

## 🚀 Quick Start

### Option 1: CSV Data Analysis
```python
import pandas as pd

# Load the comparison data
df = pd.read_csv('data/service-comparison.csv')

# Filter by service category
compute_services = df[df['Service Category'] == 'Compute']

# Find equivalent services across providers
aws_services = df[df['AWS'].notna()]
```

### Option 2: Markdown Documentation
```bash
# View the service comparison table
cat src/service-table.md
```

### Option 3: Notion Collaboration
1. Copy the content from `notion-template.md`
2. Import into your Notion workspace
3. Start collaborating with your team

## 📁 Data Structure

```
Cloud-Service-Matrix/
├── 📄 README.md                 # This file
├── 📊 data/
│   └── service-comparison.csv   # Main comparison data
├── 📝 src/
│   └── service-table.md         # Markdown version
├── 🎨 assets/
│   └── logos/                   # Provider logos
├── 📋 notion-template.md        # Notion export template
└── ⚖️ LICENSE                   # MIT License
```

## 📊 Service Categories Covered

| Category | Services | Description |
|----------|----------|-------------|
| **🖥️ Compute** | 3 | Virtual machines, containers, serverless |
| **💾 Storage** | 3 | Object, block, and file storage |
| **🗄️ Database** | 3 | Relational, NoSQL, and data warehouse |
| **🌐 Networking** | 3 | Load balancers, CDN, VPN |
| **🔒 Security** | 2 | Identity, access, and key management |
| **🤖 AI/ML** | 2 | Machine learning and speech services |
| **📈 Monitoring** | 1 | Observability and monitoring |

## 💡 Usage Examples

### Finding Equivalent Services
Looking for AWS S3 alternatives?
```csv
Service Category,Service Name,AWS,Azure,GCP,Oracle Cloud,IBM Cloud
Storage,Object Storage,S3,Blob Storage,Cloud Storage,Object Storage,IBM Cloud Object Storage
```

### Comparing Compute Services
| Service | AWS | Azure | GCP | Use Case |
|---------|-----|-------|-----|----------|
| VM Instances | EC2 | Virtual Machines | Compute Engine | Basic virtual machines |
| Container Orchestration | EKS | AKS | GKE | Managed Kubernetes |
| Serverless Functions | Lambda | Azure Functions | Cloud Functions | Event-driven computing |

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### 🆕 Adding New Services
1. Fork the repository
2. Add new rows to `data/service-comparison.csv`
3. Update `src/service-table.md` accordingly
4. Submit a pull request

### 🔄 Updating Existing Data
- Verify information from official provider documentation
- Update the "Last Updated" field
- Include source links where possible

### 📝 Guidelines
- Use official service names from providers
- Include brief descriptions for clarity
- Maintain consistent formatting
- Test CSV parsing before submitting

### 🐛 Reporting Issues
Found outdated information or missing services? [Open an issue](../../issues) with:
- Service name and provider
- Current vs. correct information
- Source documentation link

## 📈 Roadmap

- [ ] Add pricing comparison data
- [ ] Include regional availability information
- [ ] Add service maturity ratings
- [ ] Create interactive web interface
- [ ] Add more cloud providers (DigitalOcean, Linode, etc.)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Cloud provider documentation teams
- Open source community contributors
- All users who help keep this matrix up-to-date

---

**⭐ Star this repository if you find it helpful!**

**📧 Questions?** Open an issue or reach out to the maintainers.

**🔄 Last Updated**: Aug 2025
