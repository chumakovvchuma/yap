# Yap API gateway
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/youngapp/yap/blob/master/CONTRIBUTING.md) ![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/youngapp/yap/yap/master) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/570597c92b1e4ca9b67b2a49d9c2aa51)](https://www.codacy.com/gh/youngapp/yap?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=youngapp/yap&amp;utm_campaign=Badge_Grade) ![Codacy branch coverage](https://img.shields.io/codacy/coverage/e3497699cef94781936c5103f84e46ab/master) ![GitHub last commit](https://img.shields.io/github/last-commit/youngapp/yap) [![Requirements Status](https://requires.io/github/youngapp/yap/requirements.svg?branch=feature%2Fpolicies)](https://requires.io/github/youngapp/yap/requirements/?branch=feature%2Fpolicies)


Yap is the lightweight microservices API gateway that shines at the heart of any microservices or serverless architecture, which aims to be a smaller, more expressive, and more robust foundation for API management and automation workflows with low-code approach and security.

By leveraging async functions, Yap allows you to exclude callbacks and greatly improve error handling and policies at the same time providing an elegant suite of Webhook- and HTTP-based methods, which make writing servers fast and enjoyable.

Please distinguish **Yap** (the core project of Young App) and **YAP** (the platform of Young App).

## Motivation
The Young App Platform (YAP) helps to automate business workflows across cloud and on-premise apps providing employees with prompt communication and building in teams sophisticated collaboration. As an illustration, YAP automates quotes processing for cash business, which may involve multiple apps.

Without automated integration, organizations cannot leverage the full power of data in multiple applications, for example, to re-enter data in applications or constantly switch context across applications to accomplish tasks.

YAP combines the enterprise-grade workflow automation platform and ease of use expected from client apps supporting both cloud-based and on-premise systems.


## Key features of Yap
Yap offers powerful, yet lightweight features that allow fine-grained control over your API ecosystem.

* **Policies** – Policies are a powerful capability of the system that allow the publisher to change API behavior through configuration in elegants.
* **Designed for Serverless** – Yap is designed for serverless event functions on AWS, GCP or Azure Functions.
* **Connectors** – YAP is the only integration platform that was built from the ground to support a single design interface for developer/IT and for citizen integrators.
* **Universal middleware design** – Inspired by Express or KoaJS adapted for Serverless application and low-code approach.

YAP is written in NodeJS, which makes it fast and easy to set up.

## Yap API management platform
The YAP desktop version can be used with the YAP API Gateway to provide a full lifecycle API management platform. For more details, visit https://youngapp.io and to see the full feature set, explore https://manual.youngapp.co

#### Feaures available for cloud edition
* **Fully managed API** – create your API on cloud editor and hosted by Young App in realtime.
* **Advanced policies** – use advanced policies for better security.
* **Advanced connectors** – use complex app and connectors directly on the YAP platform.
* **Versioning** – use versionning for APIs and cloud processes.
* **Support and integration** – beneficiate support by experts to select the best API and cloud integration.

## Documentation

 - [Usage guide](https://manual.youngapp.co/community/usage-and-getting-started)
 - [Application and middlewares](https://manual.youngapp.co/community/application-and-middlewares)
 - [Connectors](https://manual.youngapp.co/community/connectors)
 - [Policies](https://manual.youngapp.co/community/policies)
 - [Error handling](https://manual.youngapp.co/community/error-handling)
 - [Yap for Express Users](https://manual.youngapp.co/community/faq/faq-error-policies)
 - [FAQ](https://manual.youngapp.co/community/faq/frequently-asked-questions)

## Installing
It's an official version for JavaScript, available for Node.js backends, Serverless and AWS Lambda.

##### With yarm
```
npx create yap my-api
cd my-api
yarn start
```

##### With npm
```
npx create-yap my-api
cd my-api
npm start
```

```javascript
app.post('/posts/:id', async (ctx: Context) => {
    const data = await mysql.findOne({ table: 'posts', values: { name: ctx.req.params.id } });
    ctx.body = data;
})
```

Find more details on [Usage guide](https://manual.youngapp.co/community/usage-and-getting-started)
 
## Opening issues
If you encounter a bug with YAP, we would appreciate if you inform us about it. 
Before opening a new issue, please go through [existing issues](https://github.com/youngapp/yap/issues)
to find the solution right away if your problem was solved before. 

Attach the following details if appropriate: 
- SDK, Node.js
- Environment and OS
- Stack trace
- Reduced repro case

The GitHub issues are intended for bug reports and feature requests. 
For quick help and questions on using the Yap SDK for JavaScript, please use the resources listed within [Getting Help](https://github.com/youngapp/yap#getting-help) section. The time of our support experts is rushingly flying but even so, they would like to help you in time, and therefore, will appreciate your help in applying for support reasonably by providing full details and excluding duplicated issues.

## Contribute
Yap is the open source and we love contributions! If you have an idea for a great improvement or spy an issue you’re keen to fix, follow our [Contributing Guide](https://github.com/youngapp/yap/blob/master/CONTRIBUTING.md).

No contribution is too small – we encourage you to provide feedback and [report issues](https://github.com/youngapp/yap/issues).

## License

This SDK is distributed under the GNU General Public License v3.0. 
See [LICENSE.txt](LICENSE.txt) for more information.
