# Unraid templates

Installation templates maintained by marcvandecoevering. Application code and container releases stay in their own repositories.

| App | Source and support | Container |
| --- | --- | --- |
| Dirflux (beta) | [Dirflux](https://github.com/marcvandecoevering/Dirflux) | `ghcr.io/marcvandecoevering/dirflux:beta` |
| HomeWeb | [HomeWeb](https://github.com/marcvandecoevering/HomeWeb) | `ghcr.io/marcvandecoevering/homeweb:php8.5` |

Install through Community Applications when the app is listed. For manual installation, copy the app's XML from `templates/` to `/boot/config/plugins/dockerMan/templates-user/` with a `my-` filename prefix, then select it in **Docker → Add Container**. Follow the application's installation and security instructions.

## Maintaining templates

Add one XML per application under `templates/`. Keep `Name` and `Repository` consistent with existing installations. `TemplateURL` points here; `Project`, `Support`, icons and application documentation point to the app's own repository. Validate changes in the Community Applications portal before publication.

This catalog replaces the original ThuisWeb source URL within the existing Community Applications registration; do not register it as a duplicate repository. Existing application repositories retain their old template URLs for compatibility.

HomeWeb template: MIT, see [LICENSE](LICENSE). Dirflux template: BSD-2-Clause, see [LICENSE.Dirflux](LICENSE.Dirflux). Each application retains its own license and dependencies.

The HomeWeb template retains the filename `templates/thuisweb.xml` so existing template links continue to resolve. Moving from ThuisWeb/PHP 8.3 requires an explicit image change; follow the [migration guide](https://github.com/marcvandecoevering/HomeWeb/blob/main/docs/migration.md).
