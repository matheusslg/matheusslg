### Hey there! 👋

My name is Matheus, I'm from Brazil and this is just a small resume about me. Feel free to contact me, thanks!

## <img width="45" alt="about" src="https://raw.github.com/elizarov/elizarov/master/about.png"> More about me

```js
import React, { useEffect, forwardRef, useImperativeHandle } from "react";
import PropTypes from "prop-types";

const AboutMe = forwardRef(({ newSkills }, ref) => {
  const name = "Matheus Nascimento Cavallini";
  const mainPosition = "Front-end Developer";
  const primarySkill = "React Hooks";
  const [skills, setSkills] = useState([
    "JavaScript",
    "React",
    "Angular JS",
    "Angular 2+",
    "SASS",
    "Styled Components",
    "NodeJS",
    "Git",
    "PHP",
  ]);

  useImperativeHandle(ref, () => ({
    getSkills() {
      return skills;
    },
  }));

  useEffect(() => {
    if (newSkills.length) {
      setSkills(...new Set([...skills, newSkills]));
    }
  }, [newSkills]);

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
  newSkills: PropTypes.array,
};

export default AboutMe;
```

![matheusslg's GitHub stats](https://github-readme-stats.vercel.app/api?username=matheusslg&count_private=true&show_icons=true)

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=matheusslg&hide=php&layout=compact)

[twitter]: https://twitter.com/matheus_slg
[instagram]: https://www.instagram.com/mathcavallini/
[linkedin]: https://www.linkedin.com/in/matheus-nascimento-cavallini-420408143/

#### Social Media

🐦 [twitter][twitter] **|** 
📷 [instagram][instagram] **|** 
👔 [linkedin][linkedin]

