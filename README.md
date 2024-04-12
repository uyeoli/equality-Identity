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
