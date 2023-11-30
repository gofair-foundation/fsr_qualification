# **GFF Qualification workflow for FAIR Supporting Resources (FSR)**

[TOC]

## **Introduction**

Please be aware that only qualified FIP (or 3PFF) facilitators or trainers can participate in this process. Please check this [table ](https://docs.google.com/spreadsheets/d/1hLEimbWKdlyouIF4ZoerGG6mia58c98PsVQ8hIT4hqw/edit#gid=0)if your name is already registered. 

An FSR qualification process requires **two facilitators** to quality-check new FSR nanopubs. The first facilitator acts as editor and checks if there exist more than one nanopub for the same FSR and checks the quality for the best nanopub (usually the newest) while proposing to retract the duplicates. The editor will then propose if the FSR nanopub should be accepted as is, requires changes or should be retracted. The editor assigns a reviewer, preferably one with expertise related to the FSR type, to check the action proposal for the FSR. The reviewer can accept it, request changes or reject it. If the reviewer’s answer is positive, the editor can follow the actions proposed to finally qualify it. 

There are two main procedures to take into account:

1. the functional qualification process (F steps)
2. the documentation of the technical qualification process, which is handled via git (G steps)

Both work together, as the 2) is included in the 1), documenting the actions in git. 

## **Functional qualification process - F steps**

**Overall quality-control procedure:**

**![img](https://lh7-us.googleusercontent.com/Wbst8hPCzNDMZ2-z_TYE_BwQHHoUWVVLHtasRtmvfhmhFKXdp-ZBpTEOSgxgag_yGmZeLZCJzZOFoqI9MQ5Pt8IHDBtmCa3DzVRhSN6jmjw1u1-aV5uYVVLoFQT29fXuWDgMQ5K-Mu9nzalcfPNFrMk)**

#### **Github Setup ->** [**G1 A Setup**](#g1-a-setup-steps) 

### **F1 As Editor**

A. Choose an issue from GitHub: https://github.com/gofair-foundation/fsr_qualification/issues 
   These can be filtered by label (FSR type) from https://github.com/gofair-foundation/fsr_qualification/labels 
   Assign it to you (so that everybody can see that you are working on it)

B. Check for duplicates

1. Use the API: [check duplicates](https://peta-pico.github.io/tapas/tapas.html?api=peta-pico/dsw-nanopub-api&op=/find_gofair_qualified_things_x) by searching with the most common name (and similar names) of the FSR if there exists more than one nanopub.
2. Goal is to keep only the most informative nanopub, possibly the latest one.

#### **Git Document Quality Check ->** [**G1 B**](#g1-b-steps-for-the-editor-to-document-the-quality-check)

C. Perform Quality check:

1. check if the description is informative enough or if it needs to be corrected/improved

2. check if the allocated FSR types are all correct

3. check if the links provided are working

4. check if the resource is described in FAIRsharing and if there exists a PID. If so, then check if the nanopub refers to it or if it needs to be added. Otherwise, skip it - FAIRsharing has only a few types included, so no problem if you can’t find it.

5. check the creator in publication section of the nanopub (FIP/SIP Wizard or ORCID-published in nanodash)


D. Propose action:

1. accept as is 
2. improve 
3. reject
      and assign a reviewer to check the proposal based on his/her expertise. If the reviewer doesn’t respond within 24 hours, check for another reviewer.

### **F 2 The Reviewer checks the proposal** 

and decides either to:

A. accept the proposal,
B. accept the proposal with some required changes or to
C. reject the proposal

#### **Git Document Review ->** [**G2 A**](#g2-a-steps-for-the-reviewer)

### **F3 As Editor**

- if the proposal is accepted with changes, the editor negotiates with the reviewer and makes adjustments until both are satisfied;
- if the reviewer accepts the proposal: the editor proceeds with the proposed action:

A. proposal - accept as is: qualify the FSR nanopub with the[ qualification nanopub template](https://nanodash.petapico.org/publish?12&template=https://w3id.org/np/RAleNxvRsGCSvykP0xhCSmvjS5r9UbvmmyGqEFFtbVdzc) 
B. proposal - accept with improvements: proceed with the improvement (see below)
C. proposal - reject: disapprove/retract the nanopub (see below).

D. If the reviewer rejects your proposal, get another opinion. Follow the decision that has at least two supporters;

**F 3B: Proposal accept with improvements:**

Make sure to get in contact with the creator of the FSR nanopub before you change the metadata. If you can’t get any response write an email to the creator with your intended change or, in case you don’t have the email, inform about the change in a comment directly in the FIP Wizard FSR project. 

1. If the creator is the FIP Wizard 
   1. find the project, improve the metadata and publish a new nanopub
   2. qualify the FSR nanopub with the[ qualification nanopub template](https://nanodash.petapico.org/publish?12&template=https://w3id.org/np/RAleNxvRsGCSvykP0xhCSmvjS5r9UbvmmyGqEFFtbVdzc)

2. If the creator is documented via an ORCID (then you have to work with nanodash)
   1. search for the nanopub-URI in the search of nanodash
   2. update as derived nanopublication, copy the URI of the subject in the original FSR nanopub into the short name, improve metadata and publish it
   3. in case you want to use a new template use this procedure: https://nanodash.petapico.org/publish?template=nanopubtemplateURI[&supersede=](https://w3id.org/np/RAFOJOtZQZ1dOJYAiuBf8ZZH65we0xlHWTk8G1ZFAgA68&supersede=[http://purl.org/np/RAklLUvO0mexDQmB5BRgBuRtam811bDTvGKmV0dIrWQy8)oldNanopubURI and copy the URI of the subject in the original FSR nanopub into the short name, improve metadata and publish it
   4. qualify the FSR nanopub with the[ qualification nanopub template](https://nanodash.petapico.org/publish?12&template=https://w3id.org/np/RAleNxvRsGCSvykP0xhCSmvjS5r9UbvmmyGqEFFtbVdzc)


![img](https://lh7-us.googleusercontent.com/OdLdKxfhQR5cQLdBPQFZF_K30vXsbtUvtktzV9LB-2SQKCNyIfRU2wUz5DabD-Yw3ISWQa8WRrJ_KjDnTL3frGpdG_6HzklvSpowrAOuWkeAnAqjssTqOrsIKHWcSzIh00saUEPcX8ptQDA64Ckd82Y)

**F 3C: When the FSR nanopub should be retracted:**

1. Check who is the creator: 
   1. If the creator is the FIP Wizard create a project with the Nanopublication Retraction template (under Custom templates) and follow the instructions to retract a FSR
   2. If the creator is documented with an ORCID (then you have to work with nanodash) use [this nanopub template](https://nanodash.petapico.org/publish?14&template=http://purl.org/np/RAgXKeS8wLficVpkOIbU2aF5O5Zuy7KZ_3gNUr7D5BS8c) to disapprove the nanopub (keep in mind only ORCIDs of qualified facilitators will have an impact on the FIP Wizard filters)

2. Check if same thing is described by another nanopub:
   1. If the same thing has been updated by a newer FSR nanopub (Option A), all is done
   2. If the same thing is not updated by another FSR nanopub but the entry is rejected: 
      1. Check if the FSR is used in FIPs by using this API: [**find FSRs in FIP**](https://github.com/peta-pico/dsw-nanopub-api/blob/main/tables/new_matrix_reduced.csv)
      2. Delete choice in FIP
      3. Re-publish the FIP


**![img](https://lh7-us.googleusercontent.com/m51Tu6edacZ-eimu55n_9zjAxOmYphCusaKYHKjPCqd-DFRjHiO7vXkCiRz9Ke8Q_A6vQaKmqYs7UcneG7VCdbNC4pr9qLVoZmElAbSzu4RmCsntbP1-xkii2cOVSVQe0_8rfwu-hbK-uyiTLnjMzgc)**

#### **Git Document Final Qualification steps ->** [**G1 C**](#g1-c-final-steps-for-the-editor)

## **Technical qualification workflow (documentation in github) - G Steps**

For the whole workflow we have prepared a GFF github repository to document all steps: https://github.com/gofair-foundation/fsr_qualification. The overall idea is that you should document what you do step for step. To stay on the safe side, you create for each issue a branch in github but also on your local machine. You add a new line in the csv and then you push the updated csv into the branch in github and then you open a pull request to update the main. The reviewer then reviews the pull request and will answer with a comment (to not allow it), with approval or with request changes. The editor will then actually do the changes in nanodash and finalise the documentation and close the issue and branches in github and locally.

### **Pre-requisites**

To collaborate you need a github account and we need to add your account to the FSR team (and GFF organisation) to grant write access to this repository. 

Then you should get git on your computer by downloading git from http://git-scm.com/downloads

### **G1 A Setup steps (only needed once)**

1. Create a folder on your local machine for your github repositories (e.g.: git_repo)

1. Now go to the repository on [GitHub](https://github.com/gofair-foundation/fsr_qualification): click on the green Code button and copy the URL 

![img](https://lh7-us.googleusercontent.com/iBiBYOeuDSUBI66YOP3oxsLCiQ7PNI2YFzVu0ugOTiAgYRsqBbcpqwpuWGvWwSFbJ2HrDSp8gJ9kH2poPWApE7LZ2J31tMBKyC96FZ226MolFBsyurOLsJw1y7twR6pHQlDEu7CTv3W_5t8ZJ6DFmfQ)

1. Open the command prompt window on your computer
2. To change to the folder you created: you need to use the command*:* **cd [folder]** (e.g. cd git_repo)
3. To configure your personal settings on git (needed only once) you use the command: 
   **git config --global user.name "username"**
   **git config --global user.email "email@address"**
4. To create a working copy on your computer you need to use the command*:* **git clone** **[github repo URI]** 
   (i.e. `git clone https://github.com/gofair-foundation/fsr_qualification.git`)
5. Then go to the folder that has been cloned on your computer: **cd [folder]** (e.g. cd fsr_qualification)

### **G1 B Steps for the Editor to document the Quality Check**

From the folder created above (e.g. git_repo/fsr_qualification)

1. Check that you are on the main branch: **git status**
   The output should say:
>    ```
>    On branch main
>
>    Your branch is up to date with 'origin/main'.
>
>    nothing to commit, working tree clean
>    ```

2. Ensure that you have the latest version of the spreadsheet: **git pull**

#### **Select a github issue ->** [**F1 A + B**](#f1-as-editor)

1. Create a new branch for the issue you are working on e.g.: **git checkout -b issue_353_prov**

2. Now you can directly open the *FSR_QC.csv* file in Excel (if you have problems to open the csv directly in Excel, please check these settings: First you have to make sure that in the system settings for language & region>>related settings>>administrative language setting>> format>>additional settings you have a ‘,’ . Second you need to change the setting in Excel: Go to Options >> Advanced and set a dot (.) as decimal separator) and add a new line for the FSR and add your review only in the first part (annotated in the column headers with '1.') by following the instructions in the headers. Save the file and close it.

#### **Do the quality check ->** [**F1 C + D**](#f1-as-editor)

1. In the command prompt window you need to use the command: **git status.** You should see the CSV file has been modified.
2. You now need to stage the change by using the command: **git add FSR_QC.csv**
3. **git status** should now show you that changes are ready to be committed
4. Use the command to commit it to your local repository: **git commit -m “text (e.g.added FSR qualification)”**
5. To push this to the branch you need to use the command e.g.: **git push --set-upstream origin issue_353_prov**
6. Go back to your branch on GitHub and click on contribute: **Open pull request**

*![Ein Bild, das Text, Schrift, Screenshot enthält.  Automatisch generierte Beschreibung](https://lh7-us.googleusercontent.com/s2xPCMaciIAVdkI-P8H6nlTy14EtacWymy33iePk7uP21TatUOdVip8X4iHHmpGU7m2xDZtn2M3X_ajxSlsDJIOAt-p1UADGKGmff2ehDXEJ0VfWSpPlaHgq3mmDahEUiIPDZRoQQivOBoVAKreveWE)*

1. Add in the description: **resolves #issue** 
   (Number of the issue referring to the FSR you qualified, e.g. resolves #353) 
   This links the Issue to the Pull Request.
2. Add a reviewer in the gearwear
   ![Ein Bild, das Text, Schrift, Screenshot, Reihe enthält.  Automatisch generierte Beschreibung](https://lh7-us.googleusercontent.com/Gr12xLedhmnC1QNoiWNIFlt7gy-iZFby7y0oAK2kCOBkitouS3ZnlxwNAocKQbSapqhmW88e3RjPB_Oyf5OMF7-FTJNVo2FGJOaCXbKowCXIk9N4FgbVrcX33fP1CCVrn28HJtO5PIT5q57F9j-V7UU)

And create **pull request**

### **G2 A Steps for the Reviewer**

1. You will have gotten an email alert for the pull request
2. From the pull request page, visit the branch to preview the CSV file. First, click on the branch name:



![img](https://lh7-us.googleusercontent.com/Gh_Hj89rSPTj7WxPaQoAlDyoS-FafCvSjpWJBjT2rjlJyFi3dYeLzu3kqjXMqvno2uZBy9OLZDS6u2FGuZ2QCM58eNZCyW6Ft5uCzgIMrpq_SoA5BxQJrbmzc0zQJrPo6tCPR8S4ryDOEX1-kycMEeo)

1. Then click on ![img](https://lh7-us.googleusercontent.com/95qLwETAaMCnxIiv94aO9hGH8UwTx-MRRbyUgs2I53Q8WAjsCzBBJxyVRK_1fsc6rhaNJ8JOpcKOq2BJtQYI2e_seMAkn-jWOeCMr2mCbjoAnSG7ODYkvsYvpTRspT-8v_qEolanP06UPtjI1nWu9XI) to load the preview.
2. The spreadsheet preview can be filtered if preferred by using the FSR name or NanoPub URI, e.g.:

![img](https://lh7-us.googleusercontent.com/NYrGCiqiM-Mv6IGuqh3w7HRji_se8tegbQ9Q-qQy3w4YoVteFP7rUFqXkQpRsPqrOv4TLUPb4T2tqeM7QEnVM2iUj8iM2FmCHZGXfz5mPtbJuGeUysLoSFeekfvMbtH87U5uv0YdYMijwXPLFFTeLdY)

#### **Reviewer check ->** [**F2**](https://docs.google.com/document/d/1Q0LX-5UAALDbSgLlvUvmI06ukdqHixVYO5b-9QEeFMo/edit#heading=h.zdtmx0y9xun7)

1. Review the new entry in the spreadsheet preview, this includes all columns that are named with “1. “ (at this point the “2. “ columns should be empty).
2. Make your decision on whether you approve, or request changes (or comment if you need further information or have a different opinion on the course of action).

**![img](https://lh7-us.googleusercontent.com/6OI2c-qsTeh2pcB5N0NloA4Q1smLV9dzo2Rqq0KOlh5b-YaV_d3ZVG_bhokFu9g1r4yCcwQ_NSyHxbcWe7brv5FF-WwqXvXpqBr16JHlhObqIbmPjuR7Ww1tC-pCVFP_UpcuAAesJPxci5n6XXyCnLk)**

### **G1 C Final steps for the Editor**

#### **Perform the actions ->** [**F3**](#f13-as-editor)

1. Perform the proposed actions according to the review outcome (in nanodash and FIP/SIP Wizard)
2. Use **git status** to check that you are on the correct branch
3. Open the CSV file and add your annotations in the 2nd part in the same line of the FSR to be quality checked. Save the file.
4. In the command prompt window you can use the command: **git status** to confirm that the csv has been modified.
5. Then use the command **git add FSR_QC.csv** to stage the change.
6. **git status** should show you now that changes should be committed
7. Then use the command to commit it to your local copy e.g. : **git commit -m “text (disapproved FSR nanopub)”**
8. To add this commit to the existing Pull Request you need to use the command e.g.: **git push**
10. **Merge pull request** and **confirm merge,** which closes the issue
11. Delete the branch you created on github 
12. In the command prompt: **git switch main**
    (Ensure that you do not have the CSV file open e.g. in Excel)
13. Use the command: **git pull**
14. Use the command: **git status** and you should see that you are in origin/main
15. Use the command: **git branch -d issue_353_prov** to delete the branch locally

Note: While you are waiting for the reviewer to give you feedback for your last pull request you might want to start with a new github issue. In this case you need to make sure to switch to main (11) and make a git pull (12).



------

# **Appendix A: git commands** **(in a logical order)**

| **Command** | **Purpose**                                      | **When to use it**                                           | **Example**                                                  |
| ----------- | ------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| clone       | Clone a GitHub repository into a local directory | When you want to make a copy of a repository into your local directory. | git clone https://github.com/gofair-foundation/fsr_qualification.git |
| status      | Show the status of the working tree              | When you want to see which changes have been staged, which haven't, and which files aren't being tracked by Git. | git status                                                   |
| pull        | Include changes                                  | When you want to incorporate changes from a remote repository into the current branch. If the current branch is behind the remote, then by default it will fast-forward the current branch to match the remote. | git pull                                                     |
| checkout    | Switch to a new branch                           | When you want to add a new line in the CSV, you create a new branch of main. | git checkout -b issue_353_prov                               |
| add         | *Stage* a changed file                           | When you stage a file in Git, you instruct Git to track changes to the file in preparation for a commit. | git add FSR_QC.csv                                           |
| commit      | Record changes to the repository                 | When you want to capture the state of a project at that point in time. | git commit -m “New row for PROV (issue 353)”                 |
| push        | Transfer commits                                 | When you want to upload local repository content to a remote repository. Second example also creates the new branch on GitHub. | git push  git push –set-upstream origin issue_353_prov       |
| switch      | Change to a specific branch                      | When you want to change to a specific branch                 | git switch main                                              |
| branch      | List, create, or delete branches                 | To delete an old branch for a closed issue.                  | git branch -d issue_353_prov                                 |
| diff        | Show changed files                               | When you want to see changes between two files.              | git diff                                                     |
| merge       | Integrate a development into a single branch     | When you want to incorporate changes from the named commits (since the time their histories diverged from the current branch) into the current branch. | git merge origin/main                                        |

Working with branches in git:

**![img](https://lh7-us.googleusercontent.com/f5Cx-TGT4SHZ8KNchP-q8yIdiRsWqriz0O-psOXA2w2SrrtDryejetXvotp2Dafh8aG-Ahq7Zt3TWbOSUPWhN_vvNIE_levll7LW9KO6W7AmefNVR4MHXwcrEtb_Q7aaZ_rkK03L8BfChWyYNFALUmc)**

This illustrates the need to set the upstream for `Branch_issue5` when pushing the commits from that branch.



# **Appendix B: Refreshing the GitHub issues list**

The GitHub issues list is populated from NanoDash by a custom GitHub [action](https://github.com/gofair-foundation/fsr_qualification/actions/workflows/issue.yml). 
This will create issues for new unqualified FSRs and close any open issues for FSRs that are no longer unqualified.

The action is currently unscheduled, to run it manually (e.g. after a FIP workshop): 

1. Go to the ‘Actions’ tab (red box)
2. Click on ‘issue_creation’ (blue box) 
3. Click on ‘Run workflow’ (green box)
4. Click on the ‘Run workflow’ green button (orange box)

![img](https://lh7-us.googleusercontent.com/Q_NwXiTJrHJJVxnCim_C3n1b1SMExJ-qSa153Luu14p_lHD3JYveAHBmly020Y6gx8a-N7PWiawq0bY2gzDovBxV5LuCHYmdLo8UqhuwAmBCfOc_GAXBteiTosOXozfxZq8yGvE2gGzEUBzGzXzBmLo)

![img](https://lh7-us.googleusercontent.com/Mni4rDI7AxLCDBoU-Frzn1Q3uTXZlxF-14VufHMhC056JjY7R-9qfYFlaWKEUtvs14V4vzLi_PVCU4_Eope-mo8Dk1XWwQfesGCRmJU2CHVDhDOHC_qXTij4PVVBHKSfpQK_HzJR48VRMn57rhACnzQ)
