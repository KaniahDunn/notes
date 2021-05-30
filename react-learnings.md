### React Learnings 

#### Using Font Awesome with React
First install the packages that you will need 
```
npm i --save @fortawesome/fontawesome-svg-core
npm install --save @fortawesome/free-solid-svg-icons
npm install --save @fortawesome/react-fontawesome
```

Additional packages to think about including 
```
npm install --save @fortawesome/free-brands-svg-icons
npm install --save @fortawesome/free-regular-svg-icons
```

Example code usage: 
```
import React from 'react';

import { FontAwesomeIcon } from '@fortawesome/react-fontawesome'
import { faGithub } from '@fortawesome/free-brands-svg-icons'


const ContactMe = ( ) => {
    return ( 
        <div> 
            <FontAwesomeIcon icon={faGithub} />
        </div>
    )
}

export default ContactMe;
```