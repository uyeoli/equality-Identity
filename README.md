# Title

Equality와 Identity란 무엇인가

## Equality

Equality란 객체의 동등성을 말한다.  
여기서 말하는 동등성이란 객체의 값이 같은지를 비교하는 것이다.  
동등성을 비교하기 위해서는 주로 equals()함수를 이용한다.

## Identity

Identity란 객체의 동일성을 이야기한다.  
여기서 말하는 동일성이란 객체의 메모리 주소가 같은지를 비교하는 것이다.  
동일성을 비교하기 위해서는 주로 "==" 연산자를 이용한다.

## 동등성과 동일성의 차이

의미만 봤을 때는 다르게 느껴질 수 있으나 직접 코드를 확인해보자  

![image](https://github.com/uyeoli/equality-Identity/assets/123793696/b0de72c5-05f0-4bfa-9c11-71f0b466eb99)  

Object에서의 equals함수 안에 "==" 연산자가 포함되어 있는걸 볼 수 있다.  
즉 이말은 equals는 분명 동등 비교인데 이상태로는 동일성 비교라는 것을 알 수 있다.

- 그렇다면 직접 코드로 구현해보자  

![image](https://github.com/uyeoli/equality-Identity/assets/123793696/2e2f9b55-e96c-423c-8bca-d9a55619127d)  

String은 Object를 상속받았고, 위에서 equals함수와 "==" 연산자는 똑같이 동작하는 것을 알았다. 따라서 해당 코드의 결과값은 false로 동일해야하지 않을까?  

![image](https://github.com/uyeoli/equality-Identity/assets/123793696/497d9aa7-2aa8-451c-b097-968acdd9a7ba)  

확인해보니 결과값이 다르다. 이유가 무엇일까?  

- String class에서의 equals는 Object class의 equals를 재정의 해서 사용하고 있다. 코드로 직접 확인해보자.

![image](https://github.com/uyeoli/equality-Identity/assets/123793696/4fe926da-a6aa-44ea-b6f8-12d000a37cc0)

확인해보니 Object의 equals와 String의 equals가 다르게 동작하는 것을 확인할 수 있다.  
이로 인하여 String class는 equals() 메소드를 재정의해서 주소값 비교가 아닌 문자열 '값'만을 비교한다.
따라서 equals 함수는 사용하는 객체의 특성에 맞게 재정의하여 사용을 해야 제대로 동등성의 기능을 수행할 수 있음을 알 수 있다.

##equals함수 재정의로 인한 객체의 동등성 보장

위에서는 객체의 동등성은 equals함수만 재정의하면 되는 것 처럼 보인다.






















```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc
