# Offline 3D binding

The application bundles the **PyOpenGL 3.1.9 Python package** in `PyOpenGL-3.1.9-runtime.zip`. It is imported directly on Python's module path; pip and NumPy are not required on the Raspberry Pi. The builder copies the unchanged Python package from the pinned upstream wheel, omitting its optional Windows `OpenGL/DLLS/` folder and wheel installer metadata. The installed archive contains no native binaries and remains architecture independent. The renderer uses only OpenGL 2.1 / OpenGL ES 2.0 features and system GL/EGL libraries declared in the DEB.

Source: https://pypi.org/project/PyOpenGL/3.1.9/
Wheel: https://files.pythonhosted.org (exact URL recorded by PyPI's 3.1.9 JSON metadata)
File: `PyOpenGL-3.1.9-py3-none-any.whl`
SHA-256: `15995fd3b0deb991376805da36137a4ae5aba6ddbb5e29ac1f35462d130a3f77`

The original wheel was downloaded over HTTPS and verified against https://pypi.org/pypi/PyOpenGL/3.1.9/json. The builder verifies that hash again before repacking its Python files. The source repository retains the original wheel. The installed `third-party.json` records both upstream and runtime hashes and the filtering performed. `PyOpenGL-LICENSE.txt` is the unchanged full license from the corresponding `pyopengl-3.1.9.tar.gz`, SHA-256 `28ebd82c5f4491a418aeca9672dffb3adbe7d33b39eada4548a5b4e8c03f60c8`, including its historical notices.

The OpenGL binding is the only newly bundled third-party code. Meshes, shaders, camera, shadow mapping and bounded visual contact model are original project code in `algebra_lab/qt_ui/scene3d/`. No game-engine download, generated-room image, model asset store or online rendering service is used by the new scene.
