# VeDA Verifiable Digital Assets Platform

## Inspiration

The traditional and existing digital marketplaces often fall short in establishing the verifiability and copyright of digital assets being sold. This gap inspired us to create the VeDA (Verifiable Digital Assets) Platform. Our goal is to provide creators and buyers with a marketplace that ensures peace of mind by facilitating the creation, minting, and trading of digital assets in a secure and trustworthy environment.

- **For Creators**: We aim to empower creators to confidently create and sell their digital creations, knowing their work is protected and verifiable.

- **For Buyers**: We strive to equip buyers with comprehensive information about the potential future value of the digital art they plan to purchase, allowing them to make informed decisions.

- **For Existing Digital Asset Owners**: We offer a way to identify and establish copyright for their assets, safeguarding their intellectual property.

This vision drives us to innovate and provide a platform that addresses these critical needs, fostering a more secure and reliable digital asset marketplace.

### VeDA Mind Map
![Mind Map](https://github.com/UnBoundMarketplace/documents/blob/main/diagrams/VeDAMindMap.png)
![Feature Mind Map](https://github.com/UnBoundMarketplace/documents/blob/main/diagrams/VeDAFeatureMindMap.png)

### VeDA Use Case
![Use Cases](https://github.com/UnBoundMarketplace/documents/blob/main/diagrams/VeDAUseCases.png)

## What it does

The VeDA platform provide the web3 digital arts community following functionality

- **For creators**: The platform provide following functions for our creators

    - Ability to use regenerative AI to design a digital arts collection
    - Ability to check the uniqueness of each digital arts as well as the entire collection
    - Ability to guage the average price based on past collection being sold on the platform, with project growth vectors

- **For buyers**: The platform provide following functions for our cutomers, the buyers

    - Ability to forecast the price action for a collection or a digital art piece
    - Ability to buy the digital arts
    - Ability to verify the authenticity of the digital art before buying it.

- **For exisiting owners**: The platform assist the exisiting digital arts owners, in following ways

    - Ability to check any copyright breach for the digital arts they own on the VeDA discord server
    - Ability to check if a specific digital arts if being used on discord as a profile pic without users consent

## What We Learned

Participating in the development of VeDA taught us several crucial lessons:

- **Gaps in Copyright Law**: Existing copyright laws do not adequately cover web3 digital arts, highlighting the need for new legal frameworks and protections.

- **Common Ownership Display**: The most common method for showcasing web3 digital art ownership is through social media profile pictures, known as Picture-As-Profile (PFPs).

- **Replication and Trust Issues**: Web3 digital arts are prone to easy replication and reproduction without legal repercussions, leading to devaluation and mistrust within the community.

These insights have guided our approach in creating a platform that addresses these challenges, ensuring the integrity and value of digital assets.

Participating in this hackathon has been an incredible learning experience. Here are some key takeaways:

- **Team Collaboration**: We learned the importance of clear communication and collaboration. Our team used agile methodologies to ensure everyone was on the same page.

- **New Technologies**: We explored several new technologies, including Chainlink CCIP, Functions, Discord Bot, Google Cloud Vision AI.

- **User-Centered Design**: We emphasised user experience by conducting surveys and gathering feedback, which significantly shaped our final product.

- **Time Management**: Working under tight deadlines taught us to prioritise tasks and manage our time efficiently.

## How We Built the Project

Building the VeDA (Verifiable Digital Assets) Platform involved several critical stages, from team formation to deployment. Here's a detailed account of our process:

### Team Formation and Planning

We began by identifying individuals who shared our project's goals. Our team comprised backend developers, frontend developers, UI/UX designers, and project managers. Once the team was assembled, we applied the Double Diamond design methodology to refine our idea and develop a Minimum Viable Product (MVP). The goals of the MVP were shared with the team during a comprehensive planning session.

### Project Management

To manage our project efficiently, we adopted the SCRUM methodology, conducting daily standups and iterative sprints:

- **GitHub**: Used to host repositories and manage our project via GitHub Projects.

- **CI/CD Pipeline**: Implemented to ensure all changes were tested and bug-free.

- **Communication**: Set up a Discord server for ongoing team communication.

- **Brainstorming and Design**: Utilized Whimsical for brainstorming sessions and creating UML design documents.

### Development Process

#### Initial Setup:

- **Frontend and Backend Scaffolding**: Established the basic structure for both frontend and backend projects.

- **UI/UX Design**: UI/UX designers worked on the frontend design using Figma.

#### Frontend Development:

- **Framework**: Built using Next.js for a robust and scalable frontend.

- **Deployment**: Deployed the frontend on Vercel for continuous integration and delivery.

#### Backend Development:

- **Solidity Contracts**: Developed and scaffolded using Foundry.

-  **Base Chain**: Decided to host our Solidity contracts on the Avalanche network.

- **Chainlink Functions**: Implemented for critical functionalities:

    - **Verification Function**: Utilized Google Cloud Vision AI to verify NFTs, creating a Node.js REST API to process and annotate NFT images using IPFS hashes.
      ![Verification API](https://github.com/UnBoundMarketplace/documents/blob/main/diagrams/AnalyticsAPISequenceDiagram.png)
      ![Verification API](https://github.com/UnBoundMarketplace/documents/blob/main/diagrams/VeDAAnalyticsAPIFlowchart.png)

    - **Copyright Function**: Developed to check for copyright issues, indexing Discord profiles to identify potential copyright theft through pixel comparison.
      ![Copyright API](https://github.com/UnBoundMarketplace/documents/blob/main/diagrams/VeDACopyrightFlowchart.png)

#### REST APIs:

- **Verification REST API**: This API compares the creator's digital art for uniqueness using Google Cloud Vision AI, assigning a uniqueness score and an approximate selling price. We exposed a Chainlink Function on top of this API to provide a verification data feed.

- **Copyright REST API**: This API checks if digital art owners' NFTs are being used as Discord profile pictures without consent, utilizing pixel comparison techniques.

### Integration and Testing

Once the UI/UX design was complete, we integrated the frontend with the backend services. Comprehensive end-to-end testing was conducted to ensure all components functioned seamlessly together.

### Deployment

With the integration and testing phases complete, we deployed our platform, ensuring that it was accessible and functional for users.

- The backend REST API was deployed on Google Cloud Run on Google Cloud Platform with automated Cloud Build CI/CD pipeline. 

- The solidity contract were deployed using foundry scripts

- The frontend was deployed on vercel.

- We also developed a discord bot, which was deployed on Google Cloud VM and integrated with VeDA discord server.

Challenges Faced
----------------

Throughout the hackathon, we encountered several challenges:

- Scope Creep: Initially, we had a broad vision for the project, which led to potential scope creep. We had to regularly reassess our goals and prioritize features.

- Technical Hurdles: Integrating third-party APIs, such as Google Cloud Vision AI and Discord Bot interface, for event data and ensuring cross-browser compatibility posed significant challenges.

- Team Coordination: Coordinating work across different time zones was tricky, but we overcame this with regular check-ins and flexible work hours. 

- Resource Limitations: Working with limited resources and time forced us to be creative and efficient in our problem-solving approaches.

Despite these challenges, our team's dedication and resilience enabled us to overcome obstacles and deliver a functional and impactful project.

## Accomplishments that we're proud of 

## Conclusion

Participating in this hackathon has been an enriching experience. The journey from ideation to implementation was filled with learning and growth. We are proud of what we have accomplished and look forward to continuing to develop and refine LocalEventHub to better serve our community.

## What's next for VeDA (Verifiable Digital Arts) Platform






Thank you for the opportunity to share our story!

