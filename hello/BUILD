python_sources(name="lib")

pex_binary(
    name="bin-docker",
    entry_point="main.py",
    layout="packed",
    environment="docker_linux",
)

pex_binary(
    name="bin-local",
    entry_point="main.py",
    layout="packed",
    environment="__local__",
)

docker_image(
    name="hello",
    image_tags=["local"],
    build_platform=["linux/amd64"],
)