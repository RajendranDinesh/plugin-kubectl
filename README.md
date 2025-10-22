<img src="https://cdn.rawgit.com/oh-my-fish/oh-my-fish/e4f1c2e0219a17e2c748b824004c8d0b38055c16/docs/logo.svg" align="left" width="144px" height="144px"/>

#### kubectl
> A kubectl aliases plugin for [Oh My Fish][omf-link] based loosely on the
[Oh My Zsh Kubectl Plugin][omz-kubectl-plugin].

[![MIT License](https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square)](/LICENSE)
[![Fish Shell Version](https://img.shields.io/badge/fish-v2.2.0-007EC7.svg?style=flat-square)](https://fishshell.com)
[![Oh My Fish Framework](https://img.shields.io/badge/Oh%20My%20Fish-Framework-007EC7.svg?style=flat-square)](https://www.github.com/oh-my-fish/oh-my-fish)

<br/>

## Install

```fish
$ omf install https://github.com/blackjid/plugin-kubectl
```

or with fisher

```fish
$ fisher install blackjid/plugin-kubectl
```

## Usage

### This command is used a LOT both below and in daily life

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| k            | `kubectl`                                            |

### Apply a YML file

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kaf          | `kubectl apply -f`                                   |

### Drop into an interactive terminal on a container

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| keti         | `kubectl exec -ti`                                   |

### Manage configuration quickly to switch contexts between local, dev ad staging.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kcuc         | `kubectl config use-context`                         |
| kcsc         | `kubectl config set-context`                         |
| kcdc         | `kubectl config delete-context`                      |
| kccc         | `kubectl config current-context`                     |
| kcsccn       | `kubectl config set-context --current --namespace`   |

### List all contexts

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kcgc         | `kubectl config get-contexts`                        |

### General aliases

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kdel         | `kubectl delete`                                     |
| kdelf        | `kubectl delete -f`                                  |

### Pod management.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgp          | `kubectl get pods`                                   |
| kgpa         | `kubectl get pods --all-namespaces`                  |
| kgpw         | `kubectl get pods --watch`                           |
| kgpwide      | `kubectl get pods -o wide`                           |
| kgpl         | `kubectl get pods -l`                                |
| kgpn         | `kubectl get pods -n`                                |
| kep          | `kubectl edit pods`                                  |
| kdp          | `kubectl describe pods`                              |
| kdelp        | `kubectl delete pods`                                |

### Service management.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgs          | `kubectl get svc`                                    |
| kgsa         | `kubectl get svc --all-namespaces`                   |
| kgsw         | `kubectl get svc --watch`                            |
| kgswide      | `kubectl get svc -o wide`                            |
| kes          | `kubectl edit svc`                                   |
| kds          | `kubectl describe svc`                               |
| kdels        | `kubectl delete svc`                                 |

### Ingress management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgi          | `kubectl get ingress`                                |
| kgia         | `kubectl get ingress --all-namespaces`               |
| kei          | `kubectl edit ingress`                               |
| kdi          | `kubectl describe ingress`                           |
| kdeli        | `kubectl delete ingress`                             |

### HTTPRoute management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgh          | `kubectl get httproute`                              |
| kgha         | `kubectl get httproute --all-namespaces`             |
| keh          | `kubectl edit httproute`                             |
| kdh          | `kubectl describe httproute`                         |
| kdelh        | `kubectl delete httproute`                           |

### GRPCRoute management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgg          | `kubectl get grpcroute`                              |
| kgga         | `kubectl get grpcroute --all-namespaces`             |
| keg          | `kubectl edit grpcroute`                             |
| kdg          | `kubectl describe grpcroute`                         |
| kdelg        | `kubectl delete grpcroute`                           |

### ReferenceGrant management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgr          | `kubectl get referencegrant`                              |
| kgra         | `kubectl get referencegrant --all-namespaces`             |
| ker          | `kubectl edit referencegrant`                             |
| kdr          | `kubectl describe referencegrant`                         |
| kdelr        | `kubectl delete referencegrant`                           |

### Namespace management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgns         | `kubectl get namespaces`                             |
| kens         | `kubectl edit namespace`                             |
| kdns         | `kubectl describe namespace`                         |
| kdelns       | `kubectl delete namespace`                           |

### ConfigMap management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgcm         | `kubectl get configmaps`                             |
| kgcma        | `kubectl get configmaps --all-namespaces`            |
| kecm         | `kubectl edit configmap`                             |
| kdcm         | `kubectl describe configmap`                         |
| kdelcm       | `kubectl delete configmap`                           |

### Secret management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgsec        | `kubectl get secret`                                 |
| kgseca       | `kubectl get secret --all-namespaces`                |
| kdsec        | `kubectl describe secret`                            |
| kdelsec      | `kubectl delete secret`                              |

### Deployment management.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgd          | `kubectl get deployment`                             |
| kgda         | `kubectl get deployment --all-namespaces`            |
| kgdw         | `kubectl get deployment --watch`                     |
| kgdwide      | `kubectl get deployment -o wide`                     |
| ked          | `kubectl edit deployment`                            |
| kdd          | `kubectl describe deployment`                        |
| kdeld        | `kubectl delete deployment`                          |
| ksd          | `kubectl scale deployment`                           |
| krsd         | `kubectl rollout status deployment`                  |

### Rollout management.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgrs         | `kubectl get rs`                                     |
| krh          | `kubectl rollout history`                            |
| kru          | `kubectl rollout undo`                               |
| krr          | `kubectl rollout restart`                            |

### Statefulset management.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgss         | `kubectl get statefulset`                            |
| kgssa        | `kubectl get statefulset --all-namespaces`           |
| kgssw        | `kubectl get statefulset --watch`                    |
| kgsswide     | `kubectl get statefulset -o wide`                    |
| kess         | `kubectl edit statefulset`                           |
| kdss         | `kubectl describe statefulset`                       |
| kdelss       | `kubectl delete statefulset`                         |
| ksss         | `kubectl scale statefulset`                          |
| krsss        | `kubectl rollout status statefulset`                 |

### Port forwarding

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kpf          | `kubectl port-forward`                               |

### Tools for accessing all information

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kga          | `kubectl get all`                                    |
| kgaa         | `kubectl get all --all-namespaces`                   |

### Logs

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kl           | `kubectl logs`                                       |
| kl1h         | `kubectl logs --since 1h`                            |
| kl1m         | `kubectl logs --since 1m`                            |
| kl1s         | `kubectl logs --since 1s`                            |
| klf          | `kubectl logs -f`                                    |
| klf1h        | `kubectl logs --since 1h -f`                         |
| klf1m        | `kubectl logs --since 1m -f`                         |
| klf1s        | `kubectl logs --since 1s -f`                         |

### File copy

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kcp          | `kubectl cp`                                         |

### Node Management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgno         | `kubectl get nodes`                                  |
| keno         | `kubectl edit node`                                  |
| kdno         | `kubectl describe node`                              |
| kdelno       | `kubectl delete node`                                |

### PVC management.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgpvc        | `kubectl get pvc`                                    |
| kgpvca       | `kubectl get pvc --all-namespaces`                   |
| kgpvcw       | `kubectl get pvc --watch`                            |
| kepvc        | `kubectl edit pvc`                                   |
| kdpvc        | `kubectl describe pvc`                               |
| kdelpvc      | `kubectl delete pvc`                                 |

### Daemonset management.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgds         | `kubectl get ds`                                     |
| kgdsa        | `kubectl get ds --all-namespaces`                    |
| kgdsw        | `kubectl get ds --watch`                             |
| keds         | `kubectl edit ds`                                    |
| kdds         | `kubectl describe ds`                                |
| kdelds       | `kubectl delete ds`                                  |

### CronJob management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgcj         | `kubectl get cronjob`                                |
| kgcja        | `kubectl get cronjob --all-namespaces`               |
| kgcjw        | `kubectl get cronjob --watch`                        |
| kecj         | `kubectl edit cronjob`                               |
| kdcj         | `kubectl describe cronjob`                           |
| kdelcj       | `kubectl delete cronjob`                             |

### Job management

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kgj          | `kubectl get job`                                    |
| kgja         | `kubectl get job --all-namespaces`                   |
| kgjw         | `kubectl get job --watch`                            |
| kcjj         | `kubectl create job --from=cronjob/`                 |
| kej          | `kubectl edit job`                                   |
| kdj          | `kubectl describe job`                               |
| kdelj        | `kubectl delete job`                                 |

### Events management.

| Abbreviation | Command                                              |
| ------------ | ---------------------------------------------------- |
| kge         | `kubectl get events`                                     |
| kgea        | `kubectl get events --all-namespaces`                    |
| kgew        | `kubectl get events --watch`                             |

# Credits

This was shamelessly based on on the [fish git plugin](fish-git) from [James Hillyerd](fish-git-author)

# License

[MIT][mit] © [Juan Ignacio Donoso][author] et [al][contributors]


[mit]:                https://opensource.org/licenses/MIT
[author]:             https://github.com/blackjid
[contributors]:       https://github.com/blackjid/plugin-git/graphs/contributors
[omf-link]:           https://www.github.com/oh-my-fish/oh-my-fish

[license-badge]:      https://img.shields.io/badge/license-MIT-007EC7.svg?style=flat-square
[omz-kubectl-plugin]: https://github.com/ohmyzsh/ohmyzsh/blob/master/plugins/kubectl
[fish-git]:           https://github.com/jhillyerd/plugin-git
[fish-git-author]:    https://github.com/jhillyerd
