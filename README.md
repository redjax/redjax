<h1 align="center">Thanks for visiting!</h1>

DevOps Engineer by day (and night), Linux & Open Source enthusiast by night (and day).

Writing about technology & my experiences on my [blog](https://techobyte.cc).

## My stack

###

<div align="center">
  <img src=".assets/img/linux-original.svg" height="40" alt="linux logo"  />
  <img width="12" />
  <img src=".assets/img/windows8-original.svg" height="40" alt="windows8 logo"  />
  <img width="12" />
  <img src=".assets/img/raspberrypi-original.svg" height="40" alt="raspberrypi logo"  />
  <img width="12" />
  <img src=".assets/img/python-original.svg" height="40" alt="python logo"  />
  <img width="12" />
  <img src=".assets/img/bash-original.svg" height="40" alt="bash logo"  />
  <img width="12" />
  <img src=".assets/img/powershell.svg" height="40" alt="powershell logo"  />
  <img width="12" />
  <img src=".assets/img/go-original.svg" height="40" alt="go logo"  />
  <img width="12" />
  <img src=".assets/img/azure-original.svg" height="40" alt="azure logo"  />
  <img width="12" />
  <img src=".assets/img/git-original.svg" height="40" alt="git logo"  />
  <img width="12" />
  <img src=".assets/img/docker-original.svg" height="40" alt="docker logo"  />
  <img width="12" />
  <img src=".assets/img/neovim.svg" height="40" alt="neovim logo"  />
  <img width="12" />
  <img src=".assets/img/ansible-original.svg" height="40" alt="ansible logo"  />
  <img width="12" />
  <img src=".assets/img/hugo-original.svg" height="40" alt="hugo logo"  />
  <img width="12" />
  <img src=".assets/img/jupyter-original.svg" height="40" alt="jupyter logo"  />
  <img width="12" />
  <img src=".assets/img/postgresql-original.svg" height="40" alt="postgresql logo"  />
  <img width="12" />
  <img src=".assets/img/terraform-original.svg" height="40" alt="terraform logo"  />
  <img width="12" />
  <img src=".assets/img/vscode-original.svg" height="40" alt="vscode logo"  />
  <img width="12" />
  <img src=".assets/img/cloudflare.svg" height="40" alt="cloudflare logo"  />
  <img width="12" />
  <img src=".assets/img/githubactions.svg" height="40" alt="githubactions logo"  />
  <img width="12" />
  <img src=".assets/img/netlify.svg" height="40" alt="netlify logo"  />

  <p>
    <i>More: <a href="https://github.com/redjax/Toolbelt">Toolbelt</a></i>
  </p>
</div>

## Find me on other platforms

<div align="center">
  <div style="display: flex; justify-content: center; align-items: center;">
    <a href="https://gitlab.com/redjax" style="margin-right: 24px;">
      <img src="https://raw.githubusercontent.com/redjax/redjax/feat/platform-links/.assets/img/gitlab-logo.svg" height="80" alt="GitLab"/>
    </a>
    <a href="https://codeberg.org/redjax">
      <img src="https://raw.githubusercontent.com/redjax/redjax/feat/platform-links/.assets/img/codeberg-logo.svg" height="80" alt="Codeberg"/>
    </a>
  </div>
</div>

## Notable Repositories

| Repository                                                       | Description                                                                                                                                                                                                                                                                                                                                  |
| ---------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [redkb](https://github.com/redjax/redkb)                         | My personal knowledgebase, created with [MkDocs](https://www.mkdocs.org/).                                                                                                                                                                                                                                                                   |
| [docker_templates](https://github.com/redjax/docker_templates)   | A living history of the services I have self-hosted in my homelab. Includes instructions if you want to try any of the stacks yourself. There are <!--TEMPLATE_COUNT-->175<!--END_TEMPLATE_COUNT--> templates in the repository as of <!--TEMPLATE_DATE-->2026-02-20<!--END_TEMPLATE_DATE-->.                                                |
| [Ansible](https://github.com/redjax/Ansible)                     | My Ansible monorepo, with custom roles, collections, & playbooks to manage my homelab. I use [Semaphore](https://github.com/redjax/docker_templates/tree/main/templates/automation/docker_semaphore) for orchestration.                                                                                                                      |
| [dotfiles](https://github.com/redjax/dotfiles)                   | You can tell a lot about a man by the dotfiles he keeps, & I keep mine with [chezmoi](https://www.chezmoi.io).                                                                                                                                                                                                                               |
| [PowershellProfile](https://github.com/redjax/PowershellProfile) | My `$PROFILE`.                                                                                                                                                                                                                                                                                                                               |
| [Mothership](https://github.com/redjax/Mothership)               | A "meta repository" comprised of submodules. Github Actions keep everything up to date.                                                                                                                                                                                                                                                      |
| [git_dir](https://github.com/redjax/git_dir)                     | My `~/git` directory as a repository. Handles tool installs with [mise](https://mise.jdx.dev), & uses [Taskfile](https://taskfile.dev) for automation.                                                                                                                                                                                       |
| [Terraform](https://github.com/redjax/Terraform)                 | Terraform monorepo with deployment environments. Uses [direnv](https://direnv.net) to create an environment contained to the directory, and deploys modules like [Cloudflare WAF rules](https://github.com/redjax/Terraform/actions/workflows/tf-apply-cloudflare-waf-rulesets.yml) using a Github Action. Cross-platform & well documented. |
| [system_scripts](https://github.com/redjax/system_scripts)       | Collection of scripts I have used at work & at home. The scripts are broken down by OS, then by category.                                                                                                                                                                                                                                    |

## My Homelab

I run most of my services on machines in my home and rent a VPS to serve as a reverse proxy/VPN server with identity management. Most of my sensitive services require authentication, although some are exposed to the Internet. I use Cloudflare to point my domain to the VPS, and use subdomains and a reverse proxy to route traffic over a secure tunnel back to the homelab. This way I don't have to open any additional ports on my home firewall. I block traffic using Cloudflare's WAF rules, which I manage [via Terraform](https://github.com/redjax/Terraform/tree/main/modules/cloudflare/WafZoneCustomRules).

An incomplete inventory of the hardware:

- 1 (old) blade server running Proxmox VE
  - Many VMs and LXC containers, each serving a single purpose
- 2 towers, 1 has a GPU and hosts game servers
- Multiple Raspberry Pis from different generations
- Multiple mini PCs
- Multiple rented VPSes managed by Ansible for routing and edge services
- A NAS primarily used for backup cold storage

I use [restic](https://restic.net) to backup important data, and [resticprofile](https://github.com/creativeprojects/resticprofile) to automate and organize the backups per-machine. On some server nodes, I use [backrest](https://github.com/garethgeorge/backrest) to have a web interface for managing the backups.
