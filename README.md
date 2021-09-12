### Hey there! 👋

My name is Matheus, I'm from Brazil and this is just a small resume about me. Feel free to contact me, thanks!

## <img width="45" alt="about" src="https://raw.github.com/elizarov/elizarov/master/about.png"> More about me

<img align="right" width="300" src="https://i2.wp.com/allhtaccess.info/wp-content/uploads/2018/03/programming.gif?fit=1281%2C716&ssl=1" />

```js
import React, { useEffect, forwardRef, useImperativeHandle } from "react";
import PropTypes from "prop-types";

const AboutMe = forwardRef(({ newSkills }, ref) => {
  const name = "Matheus Nascimento Cavallini";
  const mainPosition = "Front-end Developer";
  const primarySkill = "React Hooks";
  const [skills, setSkills] = useState(["JavaScript", "React", "Angular JS", "Angular 2+", "SASS", "Styled Components", "NodeJS", "Git", "PHP"]);

  useImperativeHandle(ref, () => ({
    getSkills() {
      return skills;
    }
  }));

  useEffect(() => {
    if (newSkills.length > 0) {
      setSkills(...new Set([ ...skills, newSkills ]));
    }
  }, [newSkills])

  return (
    <section>
      <h1>About me!</h1>
      <p>{`Hi, my name is ${name}, I'm a ${mainPosition} and my primary skill is ${primarySkill}.`}</p>
      <h3>Some skills:</h3>
      <ul>
        {skills.map((lng) => (
          <li>{lng}</li>
        ))}
      </ul>
    </section>
  );
});

AboutMe.propTypes = {
  newSkills: PropTypes.array
}

export default AboutMe;
```

## **GitHub Status**

<a href="https://github.com/matheusslg">
  <img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=matheusslg&theme=dracula&hide_langs_below=1" />
</a>

<a href="https://github.com/matheusslg">
 <img align="center" src="https://github-readme-stats.vercel.app/api?username=matheusslg&show_icons=true&theme=dracula&line_height=27" alt="Matheus Cavallini Github Stats"/>
</a>

[twitter]: https://twitter.com/matheus_slg
[instagram]: https://www.instagram.com/matheusslg/
[linkedin]: https://www.linkedin.com/in/matheus-nascimento-cavallini-420408143/
<br>

#### Rede Sociais!

🐦 [twitter][twitter] **|** 
📷 [instagram][instagram] **|** 
👔 [linkedin][linkedin]

