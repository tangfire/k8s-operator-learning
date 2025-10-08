```bash
[root@DESKTOP-30238IF controller-tools]# type-scaffold --kind Foo
```

```bash
[root@DESKTOP-30238IF controller-tools]# controller-gen object paths=pkg/apis/fireshine.tech/v1/types.go
```

```bash
[root@DESKTOP-30238IF controller-tools]# controller-gen crd paths=./... output:crd:dir=config/crd
```