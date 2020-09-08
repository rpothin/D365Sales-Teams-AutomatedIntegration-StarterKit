# Dynamics 365 Sales / Teams Automated Integration Starter Kit

<p align="center">
    <a href="#repolicense" alt="Repository License">
        <img src="https://img.shields.io/github/license/rpothin/D365Sales-Teams-AutomatedIntegration-StarterKit?color=yellow&label=License" /></a>
    <a href="#openissues" alt="Open Issues">
        <img src="https://img.shields.io/github/issues-raw/rpothin/D365Sales-Teams-AutomatedIntegration-StarterKit?label=Open%20Issues" /></a>
    <a href="#openpr" alt="Open Pull Requests">
        <img src="https://img.shields.io/github/issues-pr-raw/rpothin/D365Sales-Teams-AutomatedIntegration-StarterKit?label=Open%20Pull%20Requests" /></a>
</p>

<p align="center">
    <a href="#watchers" alt="Watchers">
        <img src="https://img.shields.io/github/watchers/rpothin/D365Sales-Teams-AutomatedIntegration-StarterKit?style=social" /></a>
    <a href="#forks" alt="Forks">
        <img src="https://img.shields.io/github/forks/rpothin/D365Sales-Teams-AutomatedIntegration-StarterKit?style=social" /></a>
    <a href="#stars" alt="Stars">
        <img src="https://img.shields.io/github/stars/rpothin/D365Sales-Teams-AutomatedIntegration-StarterKit?style=social" /></a>
</p>

> **Important**
> This solution used preview features (like the *Create a channel* action in flow), so it should not be used on a production environment for now.

The goal of this project is to provide to the `Power Platform community` a `kit` that will `help people automate the integration between Dynamics 365 Sales and Microsoft Teams`.

The idea behind this kit is to make the life of your Dynamics 365 Sales users easier by bringing your sales records directly in Microsoft Teams.
Microsoft Teams is now, more than ever, the collaboration hub of your company.
So, if you want to leverage collaboration to improve your sales, this starter kit will try to help you in this quest.

<p align="center">
    <a href="#solutionfeatures" alt="Solution Features">
        <img src="https://user-images.githubusercontent.com/23240245/92317829-13f23600-efd3-11ea-9e61-9b2ec069a52f.png" />
  	<figcaption>Fig.1 - Solution Features</figcaption></a>
</p>

## Prerequisites

- An environment with Dynamics 365 Sales installed
- Enable **Microsoft Teams integration** feature in the **Settings** section of the **Sales Hub** appliction
- Enable **Enable Enhanced Microsoft Teams integration (requires tenant admin permissions)** in *Settings > Administration > System Settings > General > Microsoft Teams Integration*
- An application registered in Azure Active Directory with the **Microsoft Graph** permissions below:
    - Channel.Create
    - Group.Read.All
    - TeamsApp.ReadWrite.All
    - TeamsTab.ReadWrite.All

## How to deploy the Dynamics 365 Sales / Teams Automated Integration Starter Kit?

- Import the **CustomTeamsIntegration** solution provided in the last release
- Set environment variable values
- Configure the security tab of the **MS Graph API Custom** connector
- Update the connections in each flow in the solution in the following order:
	- **Service - Get Environment Variable Value**
	- Other **Service%** flows
	- The rest of the flows
- Turn on all the flows in the solution

## Contributing to the Dynamics 365 Sales / Teams Automated Integration Starter Kit project

1. Fork this repository.
2. Create a branch: `git checkout -b <branch_name>`.
3. Make your changes and commit them: `git commit -m '<commit_message>'`
4. Push to the original branch: `git push origin <project_name>/<location>`
5. Create the pull request.

Alternatively see the GitHub documentation on [creating a pull request](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request).

## Contributors

Thanks to the following people who have contributed to this project:

<!-- Static version of the contributors list for now, but if all owners agree, we can install the AllContributors GitHub App (https://allcontributors.org/docs/en/bot/installation) 
<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center">
        <a href="https%3A%2F%2Ftwitter.com%2FRaphaelPothin">
            <img src="https://avatars.githubusercontent.com/u/23240245?v=3" width="100px;" alt=""/>
            <br />
            <sub>
                <b>Raphael Pothin</b>
            </sub>
        </a>
        <br />
        <a title="Documentation">📖</a>
    </td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

## Contact

If needed, you can contact us on twitter:
- [@RaphaelPothin on Twitter](https://twitter.com/RaphaelPothin)

## License

This project is licensed under the [MIT](https://github.com/rpothin/D365Sales-Teams-AutomatedIntegration-StarterKit/blob/main/LICENSE) license.
