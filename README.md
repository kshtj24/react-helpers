# React Helpers


### React Header Component

	import React from "react";

	const Header = ({ dark, children, className, pages }) => {
	  dark = !!dark ? "dark" : "light";
	  return (
	    <nav
	      className={
		`Header navbar navbar-${dark} bg-${dark}` +
		(className ? " " + className : "") +
		(pages && pages.length > 0 ? " navbar-expand-lg" : "")
	      }
	    >
	      <span className="navbar-brand">{children}</span>

	      {pages && pages.length > 0 && (
		<div className="collapse navbar-collapse">
		  <ul className="navbar-nav mr-auto">
		    {pages.map((item, key) => (
		      <li className="nav-item" key={key}>
		        <a href={item.Path} className="nav-link">
		          {item.Name}
		        </a>
		      </li>
		    ))}
		  </ul>
		</div>
	      )}
	    </nav>
	  );
	};

	export default Header;
	
***

### VS Code settings

[Copy this json data to settings.json in the Visual Studio Code and see the magic.](https://gist.github.com/kshtj24/ee8fdd8801822a44c9509e9cc06eab93)

***

### Important Links

#### React router
[This is the link to the react router documentation.](https://reactrouter.com/web/guides/quick-start)
#### Using OAuth Library
passport for oauth
#### HTTP status codes

#### loading other html pages
dynamic route https://gist.github.com/NMinhNguyen/e8834956acfa828821bdf2c133807dc8 
#### Bootstrap Documentation

***
