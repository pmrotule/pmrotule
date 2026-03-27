## Hi, I’m Pierre-Michel Brown 👋

### CTO & Co-founder | Software Architect | GraphQL Specialist

I am a technical leader focused on building high-performance engineering teams and resilient, scalable systems. Currently, I serve as the CTO and Co-founder of [Elio Tax](https://www.elio-tax.com) (Accès Impôt), where we are redefining tax compliance through high-scale automation and strategic AI integration.

| <a href="https://www.elio-tax.com" target="_blank"><img width="265" height="83" alt="image" src="https://github.com/user-attachments/assets/b3ae1fcb-2242-4e68-a36e-671fe39c1174" /></a> |
| :---: |
| 🇨🇦 _Online tax filing service_ 🇨🇦 |

🚀 **Growth & Experience:**
- **Scaling Expert:** Previously employee #80 at **On Running**, where I spent 7+ years helping the company scale from a local startup to a global powerhouse of 4,000+ employees.
- **Entrepreneurship:** At Accès Impôt, we double our revenue annually with an 80% customer retention rate, focusing on lean operations and technical excellence.
- **Focus:** I am dedicated to building secure, high-availability systems that thrive in an AI-transformed market. I believe that robust security and granular access control are the primary differentiators for reliable AI workflows.

---

### 🧬 Open Source Creator: GraphQL Specialization

I am the creator and maintainer of several tools designed to bridge the gap between complex data models and high-performance APIs.

#### [graphql-lookahead](https://www.npmjs.com/package/graphql-lookahead)
*An optimization utility to inspect GraphQL info objects.*
- **The Goal:** I created this to solve the N+1 problem at its root by "looking ahead" at requested fields before executing database calls, significantly reducing latency in complex graphs.

```ts
if (lookahead({ info, until: ({ field }) => field === 'product' })) {
  // include product in the query
}
```

#### [graphql-gene](https://www.npmjs.com/package/graphql-gene)
*A framework to automatically generate executable schemas from your ORM models.*
- **The Problem:** Writing redundant resolvers and keeping TypeScript types in sync is a major bottleneck.
- **The Solution:** I built `graphql-gene` to eliminate boilerplate, ensuring a single source of truth while maintaining strict type safety and high performance.

```gql
query mostRecentOrderByStatus($status: String!) {
  order(where: { status: { eq: $status } }, order: [updatedAt_DESC]) {
    id
    status
    updatedAt

    items {
      id
      price
      quantity
      product {
        name
        color

        group {
          products {
            id
          }
          categories
        }
      }
    }
  }
}
```

#### [nuxt-request-timeline](https://www.npmjs.com/package/nuxt-request-timeline)

*A performance analyzer for Nuxt.js applications.*
- **The Focus:** A specialized tool to visualize and analyze the sequence of requests during SSR or client-side navigation, helping developers identify and eliminate request waterfalls to optimize Core Web Vitals.

<img width="634" alt="Screenshot 2024-06-24 at 16 08 07" src="https://github.com/pmrotule/nuxt-request-timeline/assets/10983258/e04dad39-691f-42d5-9a5d-172e92729c4a">

---

### ⚡ Technical Toolbox

- **Languages & Frameworks:** TypeScript, JavaScript (Server & Browser), GraphQL, Vue.js, Ruby on Rails.
- **Architecture:** Microservices, Event-driven systems, Scalability & Security.
- **Cloud & Ops:** Security-first infrastructure, Automated Workflows, Continuous Deployment.
- **AI Strategy:** Leveraging LLMs to optimize internal developer velocity and external customer service.

---

### 🤝 Connect with me
- 💼 [LinkedIn](https://www.linkedin.com/in/pierre-michel-brown-34b64827b/)
- 📍 Zurich, Switzerland 🇨🇭
- 💬 Ask me about: GraphQL optimization, scaling engineering teams, or navigating the AI shift in FinTech.

*"Building for scale, coding for precision."*
