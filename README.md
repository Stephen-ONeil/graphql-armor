# GraphQL-Armor [![CI](https://github.com/Escape-Technologies/graphql-armor/actions/workflows/ci.yaml/badge.svg)](https://github.com/Escape-Technologies/graphql-armor/actions/workflows/ci.yaml)

## Supported remediations

- [x] Character Limit
- [x] Cost Analysis
- [x] Introspection

## Usage

```typescript
import { Armor } from '../src';
const armor = new Armor({});

const server = armor.apolloServer({
  typeDefs,
  resolvers,
  cache: 'bounded',
  plugins: [ApolloServerPluginDrainHttpServer({ httpServer })],
});
```
