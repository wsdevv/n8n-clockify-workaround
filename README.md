# NOTE: this version is a personal/exploratory tool
- Delete n8nr folder later, as it is a mistake

# Self Reference
Dockerfile script: 
```
# Use an official Node.js 16 image as the base
FROM node:20
RUN corepack enable

# Set the working directory to /app
WORKDIR /app

COPY (git cloned directory) custom-n8n-server

WORKDIR custom-n8n-server

WORKDIR packages/cli/bin

CMD ["n8n"]
```

![n8n.io - Workflow Automation](https://user-images.githubusercontent.com/65276001/173571060-9f2f6d7b-bac0-43b6-bdb2-001da9694058.png)

# n8n - Workflow automation tool

n8n is an extendable workflow automation tool. With a [fair-code](https://faircode.io) distribution model, n8n
will always have visible source code, be available to self-host, and allow you to add your own custom
functions, logic and apps. n8n's node-based approach makes it highly versatile, enabling you to connect
anything to everything.

![n8n.io - Screenshot](https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-screenshot.png)

## Demo

[:tv: A short video (< 5 min)](https://www.youtube.com/watch?v=1MwSoB0gnM4) that goes over key concepts of
creating workflows in n8n.

## Available integrations

n8n has 200+ different nodes to automate workflows. The list can be found on:
[https://n8n.io/integrations](https://n8n.io/integrations)

## Documentation

The official n8n documentation can be found on our [documentation website](https://docs.n8n.io)

Additional information and example workflows on the [n8n.io website](https://n8n.io)

The release notes can be found [here](https://docs.n8n.io/release-notes/) and the list of breaking
changes [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md).

## Usage

- :books: Learn
  [how to **use** it from the command line](https://docs.n8n.io/reference/cli-commands/)
- :whale: Learn
  [how to run n8n in **Docker**](https://docs.n8n.io/hosting/installation/docker/)

## Start

You can try n8n without installing it using npx. You must have [Node.js](https://nodejs.org/en/) installed.
From the terminal, run:

`npx n8n`

This command will download everything that is needed to start n8n. You can then access n8n and start building workflows by opening [http://localhost:5678](http://localhost:5678).

## n8n cloud

Sign-up for an [n8n cloud](https://www.n8n.io/cloud/) account.

While n8n cloud and n8n are the same in terms of features, n8n cloud provides certain conveniences such as:

- Not having to set up and maintain your n8n instance
- Managed OAuth for authentication
- Easily upgrading to the newer n8n versions

## Build with LangChain and AI in n8n (beta)

With n8n's LangChain nodes you can build AI-powered functionality within your workflows. The LangChain nodes are configurable, meaning you can choose your preferred agent, LLM, memory, and so on. Alongside the LangChain nodes, you can connect any n8n node as normal: this means you can integrate your LangChain logic with other data sources and services.

Learn more in the [documentation](https://docs.n8n.io/langchain/).

- [LangChain nodes package](https://www.npmjs.com/package/@n8n/n8n-nodes-langchain)
- [Chatbot package](https://www.npmjs.com/package/@n8n/chat)

## Support

If you have problems or questions go to our forum, we will then try to help you asap:

[https://community.n8n.io](https://community.n8n.io)

## Jobs

If you are interested in working for n8n and so shape the future of the project check out our
[job posts](https://apply.workable.com/n8n/)

## What does n8n mean and how do you pronounce it?

**Short answer:** It means "nodemation" and it is pronounced as n-eight-n.

**Long answer:** "I get that question quite often (more often than I expected) so I decided it is probably
best to answer it here. While looking for a good name for the project with a free domain I realized very
quickly that all the good ones I could think of were already taken. So, in the end, I chose nodemation.
'node-' in the sense that it uses a Node-View and that it uses Node.js and '-mation' for 'automation' which is
what the project is supposed to help with. However, I did not like how long the name was and I could not
imagine writing something that long every time in the CLI. That is when I then ended up on 'n8n'." - **Jan
Oberhauser, Founder and CEO, n8n.io**

## Development setup

Have you found a bug :bug: ? Or maybe you have a nice feature :sparkles: to contribute ? The
[CONTRIBUTING guide](https://github.com/n8n-io/n8n/blob/master/CONTRIBUTING.md) will help you get your
development environment ready in minutes.

## License

n8n is [fair-code](https://faircode.io) distributed under the
[**Sustainable Use License**](https://github.com/n8n-io/n8n/blob/master/LICENSE.md) and the
[**n8n Enterprise License**](https://github.com/n8n-io/n8n/blob/master/LICENSE_EE.md).

Proprietary licenses are available for enterprise customers. [Get in touch](mailto:license@n8n.io)

Additional information about the license model can be found in the
[docs](https://docs.n8n.io/reference/license/).
