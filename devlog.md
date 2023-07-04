if i don't write shit down it'll be lost forever after a few beers over the weekend

28-06-2023
notable stuff: 

fedora-iot is the platform i'm doing this all on
fetchit appuser gets a /var/home/ ~/ (idk why but i expected it to be more trad like /home/ ~)

had to create some folders after creating the app user 

sudo useradd -r -s /sbin/nologin fetchit

sudo mkdir /var/home/fetchit/.fetchit/config.yaml
sudo mkdir /var/home/fetchit/.config/systemd/user/
sudo chown -R fetchit:fetchit /var/home/fetchit/


4-07-2023
resources i've referenced so far:
* [FetchIt: Life-cycling and configuration of containers using GitOps and Podman](https://next.redhat.com/2022/08/09/fetchit-life-cycling-and-configuration-of-containers-using-gitops-and-podman/)
* [podman-kube - Play containers, pods or volumes based on a structured input file](https://docs.podman.io/en/latest/markdown/podman-kube.1.html)
* [systemd.unit — Unit configuration](https://www.freedesktop.org/software/systemd/man/systemd.unit.html)
* [make a readme.com](https://www.makeareadme.com/)