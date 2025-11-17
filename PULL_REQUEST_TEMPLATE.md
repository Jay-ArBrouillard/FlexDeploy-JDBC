  ## Pull Request Checklist

  - [ ] If Functions or Procedures are executed from outside the current package, it must be defined at the Spec level
  - [ ] If Objects are specific to the package process and are neither executed from outside nor referenced at session level, then define them at the body level ( Private objects)
  - [ ] If Objects that are referenced at a session level, it must be defined at the Spec level. (Public objects)
  - [ ] If the referenced variables, etc are used within different procedures or functions within the package, but not outside of the package, define them at the package body level.
  - [ ] Use the Pragma option when defining the function in the Package Spec as it does not perform any database updates.
  - [ ] Packages must have documentation in both Spec and Body.  When modifications are made to only the body, the documentation should be specific to the object.  If a modification is made that affects both, then the new documentation should be in both.
  - [ ] Any grants should reside in Package Spec creation script
  - [ ] Grant execute, if any procedures or functions in the package perform DML statements (insert, update, delete).
  - [ ] Package must be owned by Apps
  - [ ] Package Name should be named MAS_<SL>_NAME_PKG
