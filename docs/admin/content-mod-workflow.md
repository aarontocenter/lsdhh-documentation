# Content Moderation Workflow

The content moderation workflow affects events, job postings, and resources. 
Default moderation state is "submit for approval."

Content can be marked as being in these 5 states:
- Published
- Save as Draft
- Submit for Approval
- Archive
- Mark for Deletion

Transitions: 
- Submit for Approval: Moves content from one state to the "submit for approval" state. 
    - Published -> Submit for Approval
    - Save as Draft -> Submit for Approval
    - Submit for Approval -> Submit for Approval
    - Mark for Deletion -> Submit for Approval
- Publish: Moves content from one state to the "published" state. 
    - Submit for Approval -> Published
    - Archive -> Published
- Save as Draft: Moves content from one state to the "save as draft" state. 
    - Published -> Save as Draft
    - Save as Draft -> Save as Draft
    - Submit for Approval -> Save as Draft
- Publish this Draft: Moves content from draft to "published" state.
    - Save as Draft -> Published
- Keep Published: 
    - Published -> Published
- Archive: Moves content from one state to "archive" state.
    - Published -> Archive
    - Save as Draft -> Archive
    - Submit for Approval -> Archive
    - Archive -> Archive
- Submit for Approval: Moves content from archive to "submit for approval" state.
    - Archive -> Submit for Approval **Why isn't this part of the submit for approval above?**
- Mark for Deletion: Moves content from one state to the "mark for deletion" state.
    - Published -> Mark for Deletion
    - Submit for Approval -> Mark for Deletion
- Save as Draft: Moves content from archive to "save as draft" state.
    - Archive -> Save as Draft **Why isn't this part of the save as draft above?**