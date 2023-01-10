<h2 align="center">
  <img alt="funky" src="https://user-images.githubusercontent.com/101689311/198134861-747472e4-5380-40eb-974c-cc979681d6d1.png" width="738px"/>
<br>
<br>

  Malt Matcher is the brain-child of Cole Stephenson, where a group of 7
        developers both collaborated on, and spearheaded different ends of the
        development process to create an app that centers around something we
        are all passionate about: BEER!
</h2>

## About This Project
We worked with a React Framework on the [front-end](https://github.com/malt-matcher/malt-matcher-FE) and Ruby on Rails on the [back-end](https://github.com/malt-matcher/malt-matcher-BE), and on both sides, we implemented GraphQL to create this app to find the breweries that carried our brew of choice. The backend GraphQL API allows the client to access the full capabilities of the API data from a single end point.
  
We hope you enjoy our app while you're here! Please feel free to reach out to any of us!
 
Cheers!
  
## Backend Table of Contents 
* [Local Setup](https://github.com/malt-matcher/malt-matcher-BE/blob/main/README.md#local-setup)
* [Deployment](https://github.com/malt-matcher/malt-matcher-BE/blob/main/README.md#deployment)
* [Postman Examples](https://github.com/malt-matcher/malt-matcher-BE/blob/main/README.md#postman-examples)
* [Contributors](https://github.com/malt-matcher/malt-matcher-BE/blob/main/README.md#contributors)
## Local Setup
This project requires:
 * `Ruby 2.7.4`
 * `Rails 5.2.8.1`
### Setup Steps
 * Fork the repository
 * Clone the fork
 * Install gems and set up your database:
   * `bundle install`
   * `rails db:create`
   * `rails db:migrate`
 * Install Figaro
   * `bundle exec figaro install`
 * Update the `application.yml` file with `ENV` variables storing API keys for [Mapquest API Documentation](https://developer.mapquest.com/documentation/)
 * [Catalog Beer API Documentation](https://catalog.beer/api-docs) (No API Key required)
## Deployment 
  Interact with our live app here => https://maltmatcher.vercel.app/
## Postman Examples 

All GraphQL responses respond to POST /graphql requests only. Query information will need to be sent in the body of the request, as shown in the following GIFs.
### 1. Request/Response For Nearby Breweries That Have The Beer Style The User Is Searching For
![Nearby Breweries](https://user-images.githubusercontent.com/103782984/198139088-55ca1b46-bad0-4dc4-b390-bd2b1f9cb2d0.gif)

### 2. Request/Response For Nearby Breweries and All Of Their Beers Including The One Style Searched For
![Brewery's Beers](https://user-images.githubusercontent.com/103782984/198139523-62b0ae2c-ee70-40ed-8b84-c7af4b7d8374.gif)

### 3. With GraphQL The Front End Team Can Pick And Choose What Data They Want To See Utilizing The Same POST /graphql Request
![Pick and choose attributes](https://user-images.githubusercontent.com/103782984/198139916-2822b032-7fab-478e-b61a-0d00406052be.gif)


## Postman Demo - Nearby Brewery Beers Endpoint (Mock)
[![Run in Postman](https://run.pstmn.io/button.svg)](https://god.postman.co/run-collection/0e0f7441ce76be5d52c2?action=collection%2Fimport#?env%5Bmock%20test%5D=W3sia2V5IjoibWFsdG1hdGNoZXJVUkwiLCJ2YWx1ZSI6Imh0dHBzOi8vODljNWRhOGYtNTg3OS00YzNhLTk1OWYtMTAxZWIwOGExNzI0Lm1vY2sucHN0bW4uaW8iLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoidGV4dCIsInNlc3Npb25WYWx1ZSI6Imh0dHBzOi8vODljNWRhOGYtNTg3OS00YzNhLTk1OWYtMTAxZWIwOGExNzI0Lm1vY2sucHN0bW4uaW8iLCJzZXNzaW9uSW5kZXgiOjB9XQ==)

Follow Postman Demo Instructions Below:
```
1. Select 'Postman for Web' or 'Postman for Mac'.
2. Select a any workspace then select 'Import'.
3. Click open the 'Nearby Breweries' collection then the 'POST Get Brewery with Location and Radius' call.
4. Above the blue 'Send' button ensure 'mock test' is selected as your environment.
5. Click the 'Send' button.
6. Check out the all the fun Breweries and their Beers in the response!
7. If you click the 'body' tab (which is next to the 'headers' tab), you can checkout our GraphQL query!
```

## Technology
  <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" />  <img src="https://img.shields.io/badge/Markdown-000000?style=for-the-badge&logo=markdown&logoColor=white" />  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=Postman&logoColor=white"/> <img src="https://img.shields.io/badge/Ruby_on_Rails-CC0000?style=for-the-badge&logo=ruby-on-rails&logoColor=white" /> <img src="https://img.shields.io/badge/Ruby-CC342D?style=for-the-badge&logo=ruby&logoColor=white" /> <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" /> ![Heroku](https://img.shields.io/badge/Heroku-430098?style=for-the-badge&logo=heroku&logoColor=white) ![GraphQL](https://img.shields.io/badge/-GraphQL-E10098?style=for-the-badge&logo=graphql&logoColor=white)
  
## Database Schema
 <img alt="Schema" src="https://user-images.githubusercontent.com/101689311/198137076-f3232158-2628-4702-adf3-7af193a096b5.png" width="600px" />

## Contributors
### Back End Team
<table>
  <tr>
    <td><img src="https://avatars.githubusercontent.com/u/90064385?s=120&v=4"></td>
    <td><img src="https://avatars.githubusercontent.com/u/101689311?s=120&v=4"></td>
    <td><img src="https://avatars.githubusercontent.com/u/6260483?s=120&v=4"></td>
    <td><img src="https://avatars.githubusercontent.com/u/103782984?s=120&v=4"></td>
  </tr>
  <tr>
    <td>Parker Thomson</td>
    <td>Bryan Shears</td>
    <td>Thiago Silverira</td>
    <td>Bryce Simonds</td>
  </tr>
  <tr>
    <td>
      <a href="https://github.com/pdthomson">GitHub</a><br>
      <a href="https://www.linkedin.com/in/parker-thomson-a15a68146/">LinkedIn</a>
    </td>
    <td>
      <a href="https://github.com/b-shears">GitHub</a><br>
      <a href="https://www.linkedin.com/in/bryan-shears/">LinkedIn</a>
    </td>
    <td>
      <a href="https://github.com/tig-o">GitHub</a><br>
      <a href="https://www.linkedin.com/in/thiag-o/">LinkedIn</a>
    </td>
    <td>
      <a href="https://github.com/brycesimonds">GitHub</a><br>
      <a href="https://www.linkedin.com/in/bryce-simonds/">LinkedIn</a>
    </td>
  </tr>
</table>


### Front End Team
<table>
  <tr>
    <td><img src="https://media-exp1.licdn.com/dms/image/C4E03AQGb4Cz7abZvSA/profile-displayphoto-shrink_100_100/0/1654282848515?e=1672272000&v=beta&t=_XCHMIsfE3hviF6ywSFFxI8Un4IexbQFOWBDhFTfEa0"></td>
    <td><img src="https://avatars.githubusercontent.com/u/97558758?s=120&v=4"></td>
    <td><img src="https://avatars.githubusercontent.com/u/30582452?s=120&v=4"></td>
  </tr>
  <tr>
    <td>Cole Stephenson</td>
    <td>Jordan Farelli</td>
    <td>Andrew Miller</td>
  </tr>
  <tr>
    <td>
      <a href="https://github.com/colestephenson1">GitHub</a><br>
      <a href="https://www.linkedin.com/in/cole-stephenson-99688a240/">LinkedIn</a>
    </td>
    <td>
      <a href="https://github.com/jfarelli">GitHub</a><br>
      <a href="https://www.linkedin.com/in/jordan-farelli/">LinkedIn</a>
    </td>
    <td>
      <a href="https://github.com/andrewmiller45">GitHub</a><br>
      <a href="https://www.linkedin.com/in/andrew-miller-0393b448/">LinkedIn</a>
    </td>
  </tr>
</table>

<br></br>

![IMG_20221017_145209](https://user-images.githubusercontent.com/97558758/198148114-30fb80d6-ac60-45e1-a8da-bfe4e3069d4d.jpg)
