## WSL環境のUIの設定

- WSL環境のdevcontainerに対して、UIの設定を記述する方法
- 以下の設定を追加しておくことで、`X11`と`WAYLAND`の環境がDockerコンテナ内にも引き継がれる

``` json
{
	"mounts": [
		{"type": "bind", "source": "/tmp/.X11-unix", "target": "/tmp/.X11-unix"},
		{"type": "bind", "source": "/mnt/wslg", "target": "/mnt/wslg"}
	],
	"containerEnv": {
		"DISPLAY": "${localEnv:DISPLAY}",
		"WAYLAND_DISPLAY": "${localEnv:WAYLAND_DISPLAY}",
		"XDG_RUNTIME_DIR": "${localEnv:XDG_RUNTIME_DIR}",
		"PULSE_SERVER": "${localEnv:PULSE_SERVER}"
	}
}
```
