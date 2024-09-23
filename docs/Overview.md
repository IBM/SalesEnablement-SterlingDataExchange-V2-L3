These demonstrations assume users have at least a basic knowledge of {{offering.name}}. Before proceeding, it is highly encouraged that users complete the {{learningplan.l2}} learning plan. The plan is accessible to IBM employees <a href="https://yourlearning.ibm.com/activity/PLAN-C22C127B3AEC" target="_blank">here</a> and Business Partners <a href="https://learn.ibm.com/course/view.php?id=11891" target="_blank">here</a>.

Before proceeding, take 10 minutes to listen to Tom Limanek, B2B subject matter expert, explain the full scope of IBM B2B Integrator and some history of the many standards it supports.

![type:video](./_videos/B2BIntegratorExplained.mp4)

This demonstration solution uses the IBM Certified Containers for IBM Sterling B2B Integrator version of B2Bi. This version provides enterprise-grade and security-rich product editions with integrated common software services for consistent-deployment lifecycle management, including easy install and configure options, management of upgrade and roll-back, scalability, and security.

This course consists of four demos.

The first demo is a secure partner-to-partner data exchange solution created using IBM Sterling Business to Business Integrator (B2Bi) and Sterling FileGateway (SFG).  The setup process is detailed and fully hands on for the user to become familiar with the SterlingFIle Gateway terms such as Partner, Community, Routing Channel Template, and Routing Channel.  If the user is already familiar with SFG terms, a "Shortcut" import can be executed to save setup time. 

The second demo shows how B2B Integrator processes outbound ANSI X12 EDI files.  A set of invoices in a single batch file is pushed into a business process.  The data is split out by different receiving partners and translated into ANSI X12 "810" documents via the envelope setups and a B2Bi map.  

The third demo shows how B2B Integrator handles incoming EDI data, in this case an EDIFACT "ORDERS" document.  A key here is that B2Bi receives the document into a general mailbox that is able to process an array of EDI standards.  The process is able to determine that it is an EDIFACT document, and processes the envelope as such.   The process matches the Identifiers in the document envelopes and is able to determine a translation map to run.  The data is then translated into a "flat file" application format.  

The fourth demo focuses on Sterling FileGateway processes.  Unlike the first SFG demo, the detailed setup steps are skipped and a quicker Import process is used.  The demo shows how a zip file is sent by an "Agent" into the solution where it is unzipped, and then routed to specific directories based on the file extension. 

Learn more about B2Bi <a href="https://www.ibm.com/products/b2b-integrator" target="_blank">here</a> and access the B2Bi product documentation <a href="https://www.ibm.com/docs/en/b2b-integrator/6.1.2?topic=overview-introduction-sterling-b2b-integrator" target="_blank">here</a>. This demonstration solution uses Secure File Transfer Protocol (SFTP) to allow two partners to exchange files in a secure manner.

To create this demonstration solution, the containerized version of B2Bi will be deployed to a Red Hat OpenShift Cluster in IBM Technology Zone.

It is now time to install B2Bi on a Red Hat OpenShift cluster.
