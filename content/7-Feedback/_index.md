---
title: "7. Self Evaluation & Reflection"
weight: 7
---

> Looking back at the journey of building and deploying the PubliCast project from a local prototype to a production-ready AWS architecture, here are my personal reflections, challenges overcome, and key takeaways from the First Cloud AI Journey (FCAJ) program.

### Overall Evaluation

**1. Technical Growth & Cloud Mastery**  
Before this project, my understanding of cloud infrastructure was mostly theoretical. Through the FCAJ program, I transitioned to a hands-on approach. Designing the VPC, setting up ECS Fargate containers, and configuring Application Load Balancers gave me deep, practical insights into how large-scale systems operate.

**2. The Power of Infrastructure as Code**  
One of the most satisfying aspects was learning Terraform. Instead of manually clicking through the AWS Console, being able to define the entire infrastructure as code, destroy it, and rebuild it seamlessly was a game-changer. It taught me the importance of automation and repeatability in DevOps.

**3. Architectural Decision Making**  
The process forced me to think critically about architectural trade-offs. For instance, decoupling the monolithic backend into an API service and background workers (Worker Light/Heavy) was challenging but essential. It highlighted how to prioritize system resilience and user experience over development speed.

**4. Mentorship & Community Support**  
The support from the FCAJ mentors and the community was invaluable. Whenever I encountered complex issues—like debugging VPC S3 Endpoints or configuring CloudFront OAC—the guidance I received was prompt and encouraging. It reinforced the importance of collaborative problem-solving in tech.

---

### Key Challenges Overcome
- **Networking Complexity:** Grasping the interaction between Public/Private Subnets, NAT Gateways, and Security Groups initially felt overwhelming, but visual mapping and hands-on testing clarified the concepts.
- **CI/CD Orchestration:** Setting up AWS CodePipeline for a monorepo required precise path filtering and strict IAM roles, which was a tough but rewarding security lesson.

---

### Future Expectations
- **Next Steps for PubliCast:** I plan to expand the platform by integrating AI-driven content generation workflows and expanding the analytics dashboard.
- **Personal Goal:** To continue diving deeper into AWS Serverless technologies (Lambda, EventBridge) and pursue AWS professional certifications.

*Thank you to the FCAJ team for this incredible learning opportunity!*
