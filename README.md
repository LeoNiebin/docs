> There are two different developer tools to build either private or public integrations with on the Zapier Developer Platform: Platform UI or Platform CLI.

## Platform UI

Platform UI is the visual way for users with API experience to build integrations in a web app editor. It allows for some advanced calls and response parsing when using Code mode; but is predominantly designed for builders more comfortable with a visual form editor than working in code.

<Frame>
  <img src="https://mintlify.s3.us-west-1.amazonaws.com/zapier-82f0e938/images/a8c009d1109749b44052922f2a6ec9bc.webp" alt="Zapier Platform UI" />
</Frame>

To get started, check out the following resources:

* [Quick start guide to using Platform UI](/platform/quickstart/ui-tutorial)
* [Tutorial using Github's API to build with the Platform UI](https://community.zapier.com/featured-articles-65/zapier-platform-ui-a-complete-guide-on-how-to-integrate-with-github-26298#post108889)

## Platform CLI

Platform CLI is a terminal-based app that allows builders to scaffold new integrations locally, using standard JavaScript in your local development environment and code editor. It allows for custom coding for API calls, middleware, file support and other advanced functionality. It's the preferred tool for engineers comfortable with a standard development workflow and collaborating in a local environment using GIT version control before pushing integration versions to the Zapier server. Platform CLI can be more difficult to use for non-engineers, but will likely be more efficient for an engineering team.

<Frame>
  <img src="https://mintlify.s3.us-west-1.amazonaws.com/zapier-82f0e938/images/27d28a5fdd0c878d7558b4abd4f106ec.webp" alt="Zapier Platform UI" />
</Frame>

To get started, check out the following resources:

* [Quick start guide to using Platform CLI](/platform/quickstart/cli-tutorial)
* [Tutorial using Github's API to build with Platform CLI](https://developer.zapier.com/cli-guide/introduction)
* [CLI documentation](/platform/build-cli/overview)

## Comparison between developer tools

You can accomplish the same goals and build equally powerful Zapier integrations with both Platform UI and Platform CLI. The best tool for your integration depends on your work style and integration needs.

Below you can review what is capable between both developers tools

| Authentication         | Platform UI           | Platform CLI          |
| ---------------------- | --------------------- | --------------------- |
| Basic Authentication   | <Icon icon="check" /> | <Icon icon="check" /> |
| Session authentication | <Icon icon="check" /> | <Icon icon="check" /> |
| API Key                | <Icon icon="check" /> | <Icon icon="check" /> |
| Custom                 | <Icon icon="check" /> | <Icon icon="check" /> |
| OAuth v1               |                       | <Icon icon="check" /> |
| OAuth v2               | <Icon icon="check" /> | <Icon icon="check" /> |
| Digest                 | <Icon icon="check" /> | <Icon icon="check" /> |

| Triggers                                   | Platform UI           | Platform CLI          |
| ------------------------------------------ | --------------------- | --------------------- |
| REST Hooks                                 | <Icon icon="check" /> | <Icon icon="check" /> |
| Polling triggers                           | <Icon icon="check" /> | <Icon icon="check" /> |
| Support for static webhooks                |                       |                       |
| Customize request handling with JavaScript | <Icon icon="check" /> | <Icon icon="check" /> |

| Search Actions                             | Platform UI           | Platform CLI          |
| ------------------------------------------ | --------------------- | --------------------- |
| Search or create functionality             | <Icon icon="check" /> | <Icon icon="check" /> |
| Customize request handling with JavaScript | <Icon icon="check" /> | <Icon icon="check" /> |

| Create Actions                             | Platform UI           | Platform CLI          |
| ------------------------------------------ | --------------------- | --------------------- |
| Customize request handling with JavaScript | <Icon icon="check" /> | <Icon icon="check" /> |

| Advanced                                       | Platform UI | Platform CLI          |
| ---------------------------------------------- | ----------- | --------------------- |
| Custom middleware                              |             | <Icon icon="check" /> |
| Resources                                      |             | <Icon icon="check" /> |
| File support                                   |             | <Icon icon="check" /> |
| Hydration                                      |             | <Icon icon="check" /> |
| Import and use NPM modules                     |             | <Icon icon="check" /> |
| Organize code with common functions            |             | <Icon icon="check" /> |
| Handling long running tasks via a callback URL |             | <Icon icon="check" /> |

| Testing and Workflow               | Platform UI           | Platform CLI          |
| ---------------------------------- | --------------------- | --------------------- |
| GUI with form-based editor         | <Icon icon="check" /> |                       |
| WYSIWYG form preview               | <Icon icon="check" /> |                       |
| Write custom automated test suites |                       | <Icon icon="check" /> |
| Add team members to project        | <Icon icon="check" /> | <Icon icon="check" /> |
| Manage testers                     | <Icon icon="check" /> | <Icon icon="check" /> |
| Monitor usage                      | <Icon icon="check" /> | <Icon icon="check" /> |
| View logs                          | <Icon icon="check" /> | <Icon icon="check" /> |
| Manage versions                    | <Icon icon="check" /> | <Icon icon="check" /> |
| Use custom source code manager     |                       | <Icon icon="check" /> |
| Export integration to CLI          | <Icon icon="check" /> | -                     |

If you are still unsure after reviewing our comparsion tables, Zapier advises to build with the Platform UI.

## Switching between developer tools

### Platform UI to Platform CLI

Yes, it is possible to switch your integration from Platform UI to Platform CLI.

You can [export](/platform/manage/export-cli) an existing Platform UI integration to Platform CLI. Once exported, you can customize your integration in your local development environment. You will still have access to view your integration in the Platform UI.

Before making this change, Zapier recommends learning more about possible user impacts when [making changes to your integration](/platform/manage/planning-changes).

### Platform CLI to Platform UI

It's not possible to directly export an integration from Platform CLI to Platform UI.

You would need to create a new integration **version** built in the Platform UI (do not create an entirely new app). Existing users would most likely need to manually update their Zaps to use the new version. Learn more about [this process and best practices to minimize user impact](/platform/manage/export-ui) and contact [Developer Support](https://developer.zapier.com/contact) with any questions.

***

*Need help?* [Tell us about your problem](https://developer.zapier.com/contact) *and we'll connect you with the right resource or contact support.*
