# legacy_setuptools_compat

A bench-only helper app. Never install it on a site.

Frappe/ERPNext releases before about v15.100 import `pkg_resources` (via `dropbox`), which setuptools 81+ removed. Adding this app to a bench makes pip keep `setuptools<81` in the bench environment.

Used by the Mondaysys Cloud bench group `mondaysys-erp-v15` (erp.mondaysys.com, pinned to frappe 15.96). Remove it once that bench is on a current Frappe.
