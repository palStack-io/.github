# PalStack

> *"That's what pals do – they show up and help with the everyday stuff."*

PalStack is an open-source ecosystem of privacy-first life management tools designed to help you tackle daily tasks without sacrificing your data ownership. Self-host for free, or use our managed hosting when it launches.

## Our Services

### pantryPal
Reduce food waste and master your pantry. Track ingredients, scan receipts, integrate with recipe managers (Tandoor, Mealie), and get smart suggestions for what to cook based on what you have.

**Status:** Ready to be deployed

### finPal
Simple budget tracking that respects your privacy. Monitor spending, set goals, and understand your financial patterns.

**Status:** webUI: ready | Mobile app: 10% done

### propertyPal
Never forget home maintenance again. Track repairs, schedule recurring tasks, manage warranties, and keep your property in top shape.

**Status:** Active development

### clubPal
Coordinate group activities with rotating responsibility. Originally designed for dinner clubs, now supporting books, movies, gaming, arts, and more.

**Status:** Planning phase


## Quick Start

**Self-Hosting (Free & Open Source)**
```bash
# Clone the infrastructure repo
git clone https://github.com/palStack-io/palstack-infrastructure

# Follow the setup guide
cd palstack-infrastructure
docker-compose up -d
```

**Managed Hosting (Coming Soon)**
Premium managed hosting with automatic updates, backups, and premium features. Stay tuned!

## Architecture

- **Backend:** Python FastAPI
- **Mobile:** React Native + Expo  
- **Web:** React
- **Storage:** PostgreSQL + MinIO (S3-compatible)
- **Integration:** Home Assistant compatible

## Team

Built by a small team passionate about privacy, sustainability, and making everyday tasks easier:

- **Harun** - Founder & Lead Developer
- **Rachel Surette** - Co-Founder & Marketing, Branding & Sustainability
- **Elle Russel Chopra** - Co-Founder & Lead UI/UX Designer
- **Chris** - Co-Founder & DevOps/Systems Lead
- **Chaitanya Gunupudi** - Senior Advisor (Cybersecurity/DevOps)

## Built with AI

We openly use Claude (Anthropic) as a development assistant for prototyping, documentation, and testing. We believe in transparency about AI usage in software development.

## Documentation

- [Full Documentation](https://github.com/palStack-io/palstack-docs)
- [Self-Hosting Guide](https://github.com/palStack-io/palstack-infrastructure)
- [API Reference](https://github.com/palStack-io/palstack-docs)
- [Contributing Guidelines](.github/CONTRIBUTING.md)

## Privacy First

- **Self-hostable:** Your data stays on your infrastructure
- **Open source:** Audit the code yourself
- **No tracking:** We don't collect analytics without your consent
- **Portable:** Export your data anytime

## License

Individual services are licensed under MIT or Apache 2.0. Check each repository for details.

## Contributing

We welcome contributions! Check out our [Contributing Guide](.github/CONTRIBUTING.md) to get started.

---

**Website:** [palstack.io](https://palstack.io) (coming soon)  
**Contact:** [Contact form or email when available]
