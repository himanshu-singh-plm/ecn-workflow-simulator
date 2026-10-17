# Engineering Change Workflow Simulator

An interactive model of a PLM engineering change process (ECR, ECN, ECO), built with plain HTML, CSS and JavaScript. No install or build step.

**Live demo:** https://YOUR-USERNAME.github.io/ecn-workflow-simulator/

## What it shows
- Change lifecycle: ECR draft, ECR review, ECR approved, ECN issued, ECO in progress, released (with a reject and reopen loop)
- Role-based actions: Requestor, CCB, Change Analyst, Release Manager. Buttons are disabled unless the active role may take that step, similar to access rules in a PLM system
- Audit trail for every transition, with role and timestamp
- Data kept in the browser (localStorage); a button resets the sample data

## Why I built it
I administer Siemens Teamcenter and support Engineering Change Management in production. This project turns that process into something anyone can try in a browser.

## Notes
- All records are made-up sample data. No client or Teamcenter data is included.
- This is a simulation of the process, not a Teamcenter integration.

## Run locally
Open `index.html` in a browser.

## Ideas for next steps
- Export the audit trail to CSV
- Add affected-items and BOM impact fields
- Add a Python script that generates ECR/ECO metrics from the exported data
