```
project-root/
|-- .storybook/
|   |-- main.js
|-- app/
|   |-- (authenicated)
|   |  |-- page.tsx
|   |  |-- layout.tsx
|   |  |-- global.scss
    |-- (public)
|      |-- page.tsx
|      |-- layout.tsx
|      |-- global.scss
|   |-- page.tsx
|   |-- layout.tsx
|   |-- global.scss
|-- components/
|   |-- common/
|   |   |-- Layout/
|   |       |-- Header
|   |       |   |-- Header.tsx
|   |       |   |-- Header.module.scss
|   |       |   |-- Header.stories.tsx
|   |       |   |-- Header.test.tsx
|   |       |-- Footer
|   |           |-- Footer.tsx
|   |           |-- Footer.module.scss
|   |           |-- Footer.stories.tsx
|   |           |-- Footer.test.tsx
|   |-- features/
|       |-- Feature1Component
|           |-- Feature1Component.tsx
|           |-- Feature1Component.module.scss
|           |-- Feature1Component.stories.tsx
|           |-- Feature1Component.test.tsx
|-- clean-architecture/
|   |-- application/
|   |   |-- utils/
|   |       |-- helperFunction1.ts
|   |       |-- helperFunction2.ts
|   |   |-- useCases
|   |       |-- useCase1.ts
|   |       |-- useCase2.ts
|   |-- domain/
|   |   |-- entity1.ts
|   |   |-- entity2.ts
|   |-- infrastructure/
|       |-- api/
|       |   |-- swrConfig.ts
|       |-- repositories/
|       |   |-- entity1Repository.ts
|       |   |-- entity2Repository.ts
|       |-- state/
|           |-- jotaiConfig.ts
|-- public/
|-- styles/
|-- jest.config.js
|-- tsconfig.json
```

Explanation of the directories:

<ul>
    <li>
        <p><strong>components</strong>: Reusable UI components. Common components can be shared across different features.</p>
    </li>
    <li>
        <p><strong>app</strong>: Next.js pages. Each page file here corresponds to a route in your application.</p>
    </li>
    <li>
        <p><strong>clean-architecture/application</strong>: Contains use cases or application-specific logic. It interacts with the domain layer.</p>
    </li>
    <li>
        <p><strong>clean-architecture/domain</strong>: Represents the domain/business logic of your application. Includes entities and repositories.</p>
    </li>
    <li>
        <p><strong>clean-architecture/infrastructure</strong>: Deals with external services and configurations. In this case, it includes API configurations using SWR and state management configurations using Jotai.</p>
    </li>
    <li><p><strong>application/utils</strong>: General utility functions that can be used across the application.</p></li>
    <li><p><strong>public</strong>: Static assets like images, fonts, etc.</p></li>
    <li><p><strong>styles</strong>: CSS or styling related files.</p></li>
</ul>
