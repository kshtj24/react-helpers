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

https://www.json.org/json-en.html
https://www.kennethlange.com/rest-api-checklist/
https://www.smashingmagazine.com/2018/01/understanding-using-rest-api/
https://en.wikipedia.org/wiki/Create,_read,_update_and_delete
https://httpstatuses.com/
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Nullish_coalescing_operator
http://youmightnotneedjquery.com/
https://getbootstrap.com/docs/4.5/getting-started/introduction/
https://www.mockaroo.com/
https://github.com/praveenscience/GfG-Leadstagram/tree/Repeated-Component
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax
https://reactjs.org/docs/forms.html#controlled-components
https://github.com/praveenscience/Bootstrap-React-Helpers
https://getbootstrap.com/docs/4.5/components/navbar/
https://getbootstrap.com/docs/4.5/components/list-group/
https://reactrouter.com/
https://reactrouter.com/web/example/basic
https://github.com/praveenscience/GfG-Leadstagram/tree/Pages-Router-Demo
https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API
https://github.com/axios/axios
https://kapeli.com/cheat_sheets/Axios.docset/Contents/Resources/Documents/index
https://github.com/praveenscience/GfG-Leadstagram/tree/AJAX-States
https://developer.okta.com/blog/2019/10/21/illustrated-guide-to-oauth-and-oidc
***
