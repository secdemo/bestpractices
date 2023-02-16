# Azure App Service Should Only Allow Anonymous Access When Necessary

From **Microsoft**, [Security recommendations - Azure App Service | Microsoft Learn](https://learn.microsoft.com/en-us/azure/app-service/security-recommendations).


## Az command to check

>az webapp list --query [*].id
>az webapp auth show --ids  "/subscriptions/xxx/resourceGroups/xxx/providers/Microsoft.Web/sites/xxx" --query enabled

If result is 'false', then the AppService allows anonymous access.
