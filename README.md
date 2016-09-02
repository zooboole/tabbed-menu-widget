## How to create a pure css tabbed menu widget using radio input?

This is a tutorial on how to create a simple tabbed menu using radio input. This type of widget is widely used on website to economize space. Very useful on news websites.


<a href="https://phpocean.com/demo/tab-menu/" target="_blank">![Image of screenshot](https://phpocean.com/assets/images/source-images/pics-articles/tabdesktopimage.png)
</a>

## Install & Usage

1. Clone this reposetory or download the zip. Extract the zip in your folder.

2. Launch the `index.html` 


### Embed the code in yours

The Structure of the code is as following:

**- HTML**

* Repeat as many `tab` as the number of tabs you want for your menu
* Each radio input should have a different `id`
* Each `label` should be `for` a radio
* Mark the default **active** tab as `checked`
* In the `tab-content` you are free to put any HTML code

```
<div class="tab-wrapper">
	
	<div class="tab">
		<input type="radio" name="tab" id="tab1" checked>
		<label for="tab1">Tab One</label>

		<div class="tab-content">
			Tab content here
		</div>
	</div>

	<!-- ....... -->

</div>

```


**- CSS**

* The most important thing to keep in mind is the use of css `:checked` pseudo-class.

* Hide all input radio buttons

* The use of the css sibling selector `~` to target elements associated to a label


## Testing

You will need to test it on most common browsers. Mostly their compatibility with `:checked` pseudo-class and `~` selector.

The responsiveness can be easily handled by css `media queries`. I did an example with small devices. In that case I converted the tabs into accordion navigation.

![Image on desktop]()
![Image on mobile]()



## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.



## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
