GraphQL Pros and Cons, examples and when to use over REST

GraphQL is an open source query language developed by facebook that allows clients to formulate queries to get different results. Its main goal is to combine multiple services into one endpoint. In this video we will discuss what is GraphQL, why facebook developed it, go through some examples using github GraphQL API, finally we will discuss the pros and cons and when you should use this technology. 

- What is GraphQL? 
- Examples 
- Pros and Cons
- when to use REST vs GRAPHQL 

What is GraphQL 
- Schema
- Query language 
- Nesting
- Mutation and subscription 

Examples
Schema intro 
Github API 
Rest api 
 

Pros
- Flexibility 
- efficient response : payload back only get what you want of fields since you know the schema
- No round trips- Avoiding multiple round trips (HATEOS REST) 
- Uniform single interface API endpoint 
- Self documenting

Cons
- Complexity 
- Typed system - ( use it to know if a type is available or not and fork logic) slows down adoption.. same as soap 
- No Caching etag since always POST 
- Error management non-standard for HTTP. 
- Over engineering can lead to Inefficiency of the joins can lead to performance and DOS


https://docs.github.com/en/graphql/guides/introduction-to-graphql#discovering-the-graphql-api


WHEN TO USE GRAPHQL
Public ad-hoc API that you can’t predict how it will be used
Specific and well-design use cases API
Simple API that serves one client (webpage)
Enterprise API (new york times)
Well defined schema

Without the need of performing multiple round trips. It  as a reaction to certain limitations of the REST API. 

Schema

all post
except schema call get
 

via fetch api



Source Code for RESTAPI vs GraphQL 
https://github.com/hnasr/javascript_playground/tree/master/graphql_vs_restapi
