SCHOOL TIMETABLE — INTEGRATION REVIEW BUILD

Install: Back up original HTML, JavaScript and database. Put index.html and timetable.js in the same directory, retaining logo.jpg and logo.webp and other existing assets. Test on a separate database/project before deployment.

Changes: duplicate HTML IDs removed; current Auto-Fill modal retained; JS reference added; advanced assignment dialog replaces prompts; teacher medium fields and CSV support; day-based parallel groups; guarded single-slot swaps; lab sync; triple-period validator and task queue support.

Validation: node --check passed; HTML static duplicate-ID and inline handler-name checks passed. Browser navigation was blocked by the test environment; browser UI, Firebase synchronization, complete generator and relief integration are NOT verified.

Limitations: Advanced rules are for standalone subjects, not combined/basket subjects. Swapping individual double/triple, locked or combined slots is deliberately blocked. Lab sync skips locked/combined/parallel and already assigned slots and uses conservative room conflict checks. Weekly per-teacher quotas are not implemented. Existing authentication and database security are not redesigned; review Firebase rules and authentication separately before production.

Before deployment: test normal teaching; co-teaching; day-based; parallel medium (including day-based groups); clash prevention; workload; one/two absences; manual relief; print and export; Firebase reload and backup/restore. Existing timetable slots must be cleared for the affected subject before changing an advanced rule.
