# Microsoft Security Recommendations
[Security recommendations - Azure App Service | Microsoft Learn](https://learn.microsoft.com/en-us/azure/app-service/security-recommendations).


## App Should Enable Authentication

>az webapp list --query [*].id
>az webapp auth show --ids  "/subscriptions/xxx/resourceGroups/xxx/providers/Microsoft.Web/sites/xxx" --query enabled

If result is 'false', then the AppService allows anonymous access.
