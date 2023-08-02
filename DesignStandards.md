# 🌊 Waterfall Model
> Waterfall focuses on completeness and correctness (Quality) of the requirements before proceeding to the next phase. It is a sequential design process, often used in software development processes, in which progress is seen as flowing steadily downwards (like a waterfall) through the phases of Conception, Initiation, Analysis, Design, Construction, Testing, Production/Implementation, and Maintenance.
> This design method lends itself very well to designing Smart Contract based systems (protocols) given the immutable nature and high cost of changing the system once deployed to a public blockchain.

## (1) Analysis and Requirements Definition
1. Understand the primary goal of the system
2. Define specific requirements for the system
3. Define the scope of the system
4. Define the constraints of the system
5. Define the assumptions of the system
6. Define the risks of the system
7. Define the dependencies of the system

## (2) System Design
1. Key focus on architecture, modules, interfaces, and data for the system
2. Very important to discuss with integrators at this point to avoid costly changes later
3. Design doc should: (1) Help you organize your thoughts, (2) Solidify your point of view, (3) Rally your team around a goal, (4) Explain the why, not just the how, (5) Prevent time-sucking debates, (6) Make a developer’s life easier
4. Good documentation is all about “creating the best possible paper trail you can.” When creating design docs, include multiple design proposals, along with pros, cons, risks, and open questions for each proposal
5. Write a design that is Coordination focused: that allows you and n other engineers to coordinate your efforts; your engineering output will then be... "I coordinated a team to build something that any of us couldn't have written individually."

## (3) Implementation
> Use a top-down approach for coordinating and assigning tasks: Start with breaking down the primary goal into smaller goals and break those goals into even smaller goals. Do this with parallelism in mind. Organization can be done via Github tasks or some other management tool. 
> Smaller goals at the engineering level may also require a degree of design and documentation. This is fine and should be encouraged if the task is complex enough to warrant it.
1. Test Driven Development (TDD) is encouraged
2. Documentation in Waterfall is done across all phases but is emphasized in this phase
3. **(3) Implementation** and **(4) Testing** are often done concurrently; *do not* wait until a feature is fully implemented before testing it

## (4) Testing
1. Unit Testing (fuzzing, etc.) **(done *in parallel* with implementation)**
2. Integration Testing **(done *in parallel* with implementation)**
3. System Testing **(done *in parallel* with implementation)**
4. Invariant and other advanced forms of testings **(done *post* implementation)**
5. Formal Verification **(done *post* implementation)**

## (5) Audits
1. Establish common understanding of the system with auditors
2. Ensure that the system is built according to the requirements
3. Ensure that the system is built according to the design
4. Step (1) "Analysis and Requirements Definition" should be communicated clearly and shared with auditors

## (6) Deployment
> All deployments should be verified on Etherscan and other relevant block explorers
1. Testnet Deployment
2. Mainnet Deployment
3. Update documentation and other *public* resources with relevant information (addresses, etc.)

## (7) Maintenance (upgrades, etc.)
> All upgrades should be verified on Etherscan and other relevant block explorers
1. Testnet upgrades are crucial to ensure there are no state collisions which are catastrophic to the system
2. If possible, A/B testing (also known as split testing or bucket testing) can be incredibly valuable

#### Further Reading
1. [Waterfall Model](https://en.wikipedia.org/wiki/Waterfall_model)
2. [How Dropbox Designs a Design Doc](https://medium.com/dropbox-design/how-do-you-design-a-design-doc-d7b2f1fa4a0c)
3. [Ycombinator: Design Docs at Google](https://news.ycombinator.com/item?id=23915521)
4. [HUIT Enterprise Project Management Office​](https://pmo.huit.harvard.edu/methodology-framework%E2%80%8B)