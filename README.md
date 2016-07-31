# rails-alpine

Rails environment built with alpine-linux, openssh, git, and other dependencies.

based on the offical Ruby Image: [ruby:alpine](https://hub.docker.com/_/ruby)

### [IMPORTANT For 5.0.0]: 

!!!!`bluebu/rails-alpine` the rails version will be upgrade to `5.0.0` on `2016-08-15` 

 Please use the `bluebu/rails-alpine:rails4` tag in repace,  if you are still using Rails 4.2.x 


### Usage:

~~~
docker pull bluebu/rails-alpine

docker pull bluebu/rails-alpine:rails5

docker pull bluebu/rails-alpine:2.2-rails4
~~~

### Tags & Versions:
 
| Tags            | Ruby Ver.     | Rails Ver.    | 2016-08-15*   |
| :-------------  |:-------------:| ------------- | ------------- |
| latest          | 2.3           | 4.2.7         | 5.0.0*        |
| 2.3             | 2.3           | 4.2.7         | 5.0.0*        |
| 2.2             | 2.2           | 4.2.7         | 5.0.0*        |
| 2.1             | 2.1           | 4.2.7         | 5.0.0*        |
| rails5          | 2.3           | 5.0.0         |               |
| 2.3-rails5      | 2.3           | 5.0.0         |               |
| 2.2-rails5      | 2.2           | 5.0.0         |               |
| 2.1-rails5      | 2.1           | 5.0.0         |               |
| rails4          | 2.3           | 4.2.7         |               |
| 2.3-rails4      | 2.3           | 4.2.7         |               |
| 2.2-rails4      | 2.2           | 4.2.7         |               |
| 2.1-rails4      | 2.1           | 4.2.7         |               |

*The tags will be upgraded to rails5 when 2016-08-15