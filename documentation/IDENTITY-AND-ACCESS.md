# Identity and access model

**Domain:** `Smallville.local` (specified for the student in the course scenario).

**Departments:** Human Resources, Marketing, Sales. Each department has four users and one manager in the assignment design.

**Proposed permission architecture:** Accounts → department global groups → resource domain-local groups → NTFS permissions (AGDLP). Department users need to add/edit files but must not delete documents; managers can add/edit/delete only within their own department. Windows permissions for edit-without-delete require careful advanced NTFS permission design and testing; do not assume a generic `Modify` grant meets this requirement.

The worksheet includes HR group membership screenshots and some file permission views. Other department group screenshots are not equally complete; consult the evidence gallery before making broader completion claims.
