# opencode-template

This helm chart deploys a opencode environment running within Red Hat DevSpaces running on OpenShift.

## Models
There are a number of models providers configured:

1. OpenCode
1. Red Hat Models as a Service
1. Red Hat LLama Stack
1. OpenRouter provided models

Their URLs and API keys are configured in the values.yaml file

## MCP Servers
There are three configured MCP Servers :

1. Context7 for code documentation searching
1. Github Grep  https://vercel.com/blog/grep-a-million-github-repositories-via-mcp
1. Remote Skills MCP server - https://github.com/noelo/claude-skills-mcp

## Base Container

The base container contains the following tools


|Command           | Version          | Name         |
|------------------|------------------|--------------|
|oc                |4.20.3            |OpenShift CLI |
|kubectl           |1.33.3            |Kubernetes CLI|
|kustomize         |5.8.0             |Kustomize CLI |
|helm              |4.0.1             |Helm CLI      |
|jq                |1.8.1             |jq            |
|python            |3.12.11           |python        |
|node              |22.19.0           |Nodejs        |
|bash              |5.2.26            |bash          |
|argocd            |3.2.0             |ArgoCD CLI    |
|yq                |4.49.1            |yq            |
|opencode          |                  |OpenCode      |


The containerfile is at https://github.com/noelo/web-terminal/blob/main/Containerfile

## How to use

Open a terminal by pressing the keys "ctrl-shift-c" and then type "opencode"