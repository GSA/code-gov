
This document is to memorialize internal project procedures.  Other agencies or teams not at GSA are free to adopt them as well, but don't have to in order to use the software.  

### Cloud.gov Access 

The System owner and current project developers need cloud.gov access to the code.gov API.  The system owner (currently Joe Castle) manages this access, granting access to new project developers when they come onboard and removing access when they leave.  

Specifically, current developers are [granted](https://cloud.gov/docs/apps/managing-teammates/) OrgManager rights to `gsa-code-gov` and SpaceDeveloper rights to each of the projects spaces.    

These accounts are created for developers that need access to contribute code and debug apps.  The system owner will send an invite from Cloud.gov to the new users GSA government email address.

1. [Create an account](https://cloud.gov/) with Cloud.gov from the invite. This will need to include multi-factor authentication with [Google authenticator](https://support.google.com/accounts/answer/1066447?hl=en) or [authy](https://www.authy.com/).

2. Make sure you have [gitseekrets](https://github.com/18F/laptop/tree/master/seekret-rules) installed on your Mac or in your virtualbox, if that is where you do your development. 

3. Then, you will want to contact the system owner, currently Joe Castle.  In that message, confirm you have two factor authentication on and have installed gitseekrets. 

4. The system owner will confirm the GSA identity of the applicant and add a person to the `gsa-code-gov` organization in cloud.gov. 
 
6. Documenting what role was assigned.

### GitHub Access 

The System owner and current project developers need commit rights to code.gov project repositories. The system owner manages this access, granting access to new project developers when they come onboard and removing access when they leave.  

These accounts are created for developers that need access to contribute code and deploy apps.

1. [Create an account](https://github.com/) with GitHub and [enable multi factor authentication](https://github.com/blog/1614-two-factor-authentication).
2. Make sure you have [gitseekrets](https://github.com/18F/laptop/tree/master/seekret-rules) installed on your Mac or in your virtualbox, if that is where you do your development. (If you are a Windows only user, you can be exempt from this requirement while the windows version is in development.) 
3. Then, you will want to contact the system owner. In that message, include your name, the name of your supervisor, confirm you have two-factor authentication on and have installed gitseekrets. 
5. The system owner will then send a request to gsa-github.support@gsa.gov to add the user to the GSA org on GitHub. Once that is complete the system owner wll them add them to the GSA/code-gov and GSA/code-gov-dev-team GitHub teams.

### Weekly Monitoring Checklist

The development team checks for security events weekly. These checks are logged in a Trello card.
Any unusual or suspicious activities are immediately brought to the team's attention in the project slack channel (#code-gov-partners) and the system owner coordinates appropriate investigation and followup. The team will follow the [18F incident response handbook](https://handbook.18f.gov/security-incidents/).

Checklist:
1. Create an issue in the project's issue tracker to track this Security Event Review.
2. Review New Relic for all alerts flagged with 'red' flags.

3. Review [production logs](https://logs.fr.cloud.gov) for unapproved and unusual activities. 
4. Review actionable security events on production logs for successful and unsuccessful account logon events, account management events, object access, policy change, privilege functions, process tracking, system events, all administrator activity, authentication checks, authorization checks, data deletions, data access, data changes, and permission changes.
5. Deactivate any cloud.gov and GitHub access for people who have left the team.
6. Note any findings in the Security Event Review issue.
7. Close the Security Event Review issue.

### Monitoring of New Relic Alerts


[New Relic alerts](https://rpm.newrelic.com/accounts/1651802/applications) are emailed to the full development team immediately.  The first team member to see the alert checks the site's status and posts in the project slack channel (#code-gov-partners) the results.  The system owner then coordinates any necessary followup.  

