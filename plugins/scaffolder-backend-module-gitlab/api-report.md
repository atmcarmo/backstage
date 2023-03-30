## API Report File for "@backstage/plugin-scaffolder-backend-module-gitlab"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { JsonObject } from '@backstage/types';
import { ScmIntegrationRegistry } from '@backstage/integration';
import { TemplateAction } from '@backstage/plugin-scaffolder-node';

// @public
export const createGitlabProjectAccessTokenAction: (options: {
  integrations: ScmIntegrationRegistry;
}) => TemplateAction<
  {
    repoUrl: string;
    projectId: string | number;
    name: string;
    accessLevel: number;
    scopes: string[];
    token?: string | undefined;
  },
  JsonObject
>;

// @public
export const createGitlabProjectDeployTokenAction: (options: {
  integrations: ScmIntegrationRegistry;
}) => TemplateAction<
  {
    repoUrl: string;
    projectId: string | number;
    name: string;
    username: string;
    scopes: string[];
    token?: string | undefined;
  },
  JsonObject
>;

// @public
export const createGitlabProjectVariableAction: (options: {
  integrations: ScmIntegrationRegistry;
}) => TemplateAction<
  {
    repoUrl: string;
    projectId: string | number;
    key: string;
    value: string;
    variableType: string;
    variableProtected: boolean;
    masked: boolean;
    raw: boolean;
    environmentScope: string;
    token?: string | undefined;
  },
  JsonObject
>;
```