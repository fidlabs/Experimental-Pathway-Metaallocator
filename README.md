# Experimental Pathway Metaallocator

Contact: @DamianPudlo on Filecoin Slack

## **Summary**
This proposal introduces an **Experimental Pathway Metaallocator (EPMA)** within the Filecoin Plus (Fil+) program, designed for allocators that seek to experiment with novel approaches to making DataCap (DC) allocations. This initiative recognizes that teams need access to DC to test new allocation mechanisms and aims to provide a structured yet flexible environment for experimentation while minimizing the risk of abuse. **The proposal is made by FIDL team and FIDL proposes to manage the EPMA.**
### Preface



In the rest of the document “Applicant” designates a team or an individual submitting the application. The unique ID of the application consists of who applied and what was the idea.



## **Key Rules**
1. **Eligibility**: Only applicants proposing a new evaluation metric (e.g. not demonstrating value to the network through existing evaluation metrics) are eligible to apply.  
2. **Allocation Limit**: A maximum of **1 PiB of DC** can be granted to any individual applicant.  
3. **Transition Requirement**: By the time an allocator exhausts its 1 PiB DC, it is expected that they will be ready to apply as a direct allocator or within a meta-allocator pathway evaluating their success.  
4. **Reapplication Policy**:  
  * In very rare occasions, applicants can only reapply for an extension **once after 6 months**.  
  * To reapply, they must submit a **detailed progress report** on their allocation model, including insights gained, challenges faced, and a justification for why they require additional DC rather than transitioning to an established allocation pathway.  
5. **Adherence to plan:** Applicants who do not continue diligence operations via the methodology of their experimental pathway, will not be onboarded as Manual pathways.

## **Objectives**



* Encourage the development of innovative allocation mechanisms by lowering the entry barrier for experimental allocators.  

* Automate the process making application and tracking more efficient.  

* Introduce safeguards to prevent misuse of experimental allocations as a shortcut to free DC.



## **Process**



### Application



An allocator wishing to obtain DC through this pathway will need to submit an application using an online application form and provide the following information:



1. Details of team or individual that is applying:
   1. Name(s).
   2. Country(ies) of residence.
   3. Github Account(s) of the applicant(s).
   4. Slack Name(s)/Unique Slack ID(s).
   5. Email(s).  
2. Description of the experiment intended, including:
   1. Detailed description of automation used.
   2. Expected allocation schedule.
   3. Duedilligence or other methods of abuse prevention.
   4. Expected results.
   5. Definition of success.
   6. Metrics measuring the success/failure (OKRs or similar).
   7. Milestones or development plan  
3. Github repository with an active development history demonstrating work on an allocation model.  
4. Onchain wallet to receive DC.  
5. Name of the entity that will be performing audit of the code upon the maturation of the experiment. 

### Review  
Once application is received, the EPMA will:
1. Review the content of GitHub repository, analyzing the commit history and contributor activity using to ensure consistent and genuine development efforts.  
2. Automatically detect potential duplicates or plagiarism of the codebase.  
3. Request a KYC from the applicant and perform sanction checks  
4. Verify that the applicant has not received DC within the last 6 months for the same or similar project.  
Provided that the above checks are passed, the applicant will receive 1PiB of DC to the wallet they provided in the application.

### Maturation
The project is ready to move to maturation phase in one of two cases:
1. The experiment is successful and the system works as proposed.  
2. The experiment failed and the proposed method cannot be used to allocate DataCap. 
In either case the applicant is expected to submit a report, in order to help the community grow. The report should contain:
  1. The hypothesis
  2. The model intended
  3. Gained insights
  4. Challenges faced
  5. Conclusions and proposals for further improvements.
  6. Additionally:
     1. In case of failed experiments, the applicant should include a post-mortem reasoning of why the experiment failed
     2. In case of success, the applicant should include a full audit report delivered by the auditor included in the initial application. (In rare cases, the applicant may request to change the auditing team, but this must be approved by the Experimental Pathway Meta Allocator team beforehand). 
These artifacts will be reviewed by the EPMA team and, provided the experiment was successful and the maturation report passes the review, the EPMA team will support the applicant in launching an Allocator.
## **Principles**
To determine whether an applicant is genuinely developing an allocation system rather than simply acquiring free DC, we propose the following evaluation criteria:
1. **Code Repository Requirement**  
  Applicants must provide a public repository with an active development history demonstrating work on an allocation model. This will be verified through GitHub API: Check for commits, PRs, and activity over a prior 3 months. Realizing that a lot of the development may rely on the DC allocation, the activity in GitHub can be development of the proposal and written documents, rather than code. Although code will be a plus.  
2. **Automated Performance Metrics**  
  Metrics such as allocation speed, distribution diversity, and compliance with Fil+ policies can be periodically checked.  
3. **Ongoing documentation of the progress**  
  In addition to code development, the GitHub repository should contain documentation of the ongoing development. This should include:
* The hypothesis
* Detailed description of automation used.
* Failures and successes so far.
* Ongoing reporting on the developments, including:
*  Failures and successes so far.
*  Documentation of approaches so far
*  Progress on the OKRs from the application
*  Milestones achieved so far.
*  Duedilligence or other methods of abuse prevention.  
4. **Audit**  
  Every applicant has to submit details of a third party auditor which (upon the successful development of the allocator) will perform code audit that verifies  
    1. Security of the code  
    2. Whether the code is doing what the applicant intended in their application  
    3. Does it prove the hypothesis submitted in the application  
  _Upon maturation, in order to move to the next phase and launch the allocator, the audit report must be submitted and verified by the EPMA team._  

5. **Duplicates and Plagiarism**  
  If an application is found to be a duplicate of another application, vastly similar to the already proposed approach or not novel in some other way, it will be automatically rejected. Applicants making repeated failing applications will be banned from applying to the EPMA for lifetime.  

6. **Secret Shopper Test**  
  The EPMA team will conduct secret shopper experiments to verify that the experiment is working as intended. Failing the test will cause immediate removal from the program. 
