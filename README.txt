Public PostgreSQL/PostGIS pilot image

Proposed package: ghcr.io/edufelip/guiabrecho-postgis17:pg17.11-postgis3.6.4-pilot-20261003
This repository contains public database software publishing material only. It contains no application source/JAR, application database schema/dump, user data or credentials.

The publisher loads a qualified archive without rebuilding. Archive SHA256 d6d1fc27e028ff97948ff47ebd79f5b978a34d92fef20ed32735187bc6897621, bytes190244842. Local OCI manifest f8b30b7c3516023f4fbf9f786ba663e2fe7acf9adc757b7f89ac0e500eb58f4d; runtime configuration 7133289958adf16e71ebef053e4921b9b2f2012ae5ab31bc46f12929ba1958cd. These are archive/local bindings, not a claimed independently verified published GHCR digest.

PostgreSQL17.11, PostGIS3.6.4, Alpine3.24.1. Maintainer base linux/amd64 manifest7ce143dbc804dc08a8f1dcf9067724f9b6e4ded48711e9d884487967acb442b3 from postgis/postgis. Official same-suite package updates: libexpat2.8.5-r0, pcre2 10.49-r0, libuuid2.42.3-r1. SQLite3.53.4-r0 and libxml2 2.13.9-r2 retained. No custom distro security fork.

Gosu1.19 source commit6456aaa0f3c854d199d0f037f068eb97515b7513 built with Go1.27.1; binary SHA2569ebd2c978d2a66aeee22a52a0679f0351ad72eb0cb7b61c4ee3e21a0ccc52f48. Copies of the exact retained gosu/Go/moby-user/x-sys notices are in notices/. PostgreSQL/PostGIS and distribution package licenses retain their respective original terms; no claim that this entire image has one license.

Source and license references:
https://github.com/postgis/docker-postgis
https://github.com/postgis/postgis/tree/3.6.4
https://www.postgresql.org/ftp/source/v17.11/
https://gitlab.alpinelinux.org/alpine/aports/-/tree/3.24-stable
https://github.com/tianon/gosu/tree/6456aaa0f3c854d199d0f037f068eb97515b7513
https://go.dev/dl/#go1.27.1

Security limitation: libxml2 2.13.9 remains in upstreamCVE-2026-86138's affected range below2.15.4; other manually identified XML advisories require individual dispositions. A local unfiltered Trivy0.75.0 scan reported0CRITICAL/0HIGH,4MEDIUM,6LOW,3UNKNOWN; this is not comprehensive vulnerability clearance. Follow supported vendor patches and requalify replacements.
