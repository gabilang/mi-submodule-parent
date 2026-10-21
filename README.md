# mi-submodule-parent

Micro Integrator project used to verify git submodule checkout in MI builds on the integration platform.

- `src/main/wso2mi/artifacts/apis/HelloWorldAPI.xml`: `GET /hello/world` returns a fixed greeting.
- `lib/`: git submodule (`submodule-fixture`), pinned to its first commit. It is not part of the Maven build; the checkout step's log shows which commit it was checked out at.
- `project.runtime.version` in `pom.xml` selects the MI runtime (4.4.0). A `MI_VERSION` build environment variable overrides it.
# mi-submodule-parent
