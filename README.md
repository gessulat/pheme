With Pheme you can compare predictions against some ground truth visually. Visualizations are specific to the data type of the prediction. Currently available data types are:
test

- mass spectra


![screenshot](https://raw.githubusercontent.com/gessulat/pheme/master/images/pheme.jpg)

---
# Installation

You need to install:

- Node + npm
- polymer-cli with `npm install -g polymer-cli`

Running the app.

- The first time startin the app, run `bower install` in the main directory.
- Start the app with `polymer serve -o`.

---

## Data Specification
Data for all types needs to be provided in .json as follows.

**Dataset Specification**
        
        
	dataset: {
	    phemeType: 'mass_spectrum',
	    samples: [
	        {   meta: { },
	            data: { target: [], prediction: [] }
	        },
	    ],
	},


**Data Sample Specification**

 `prediction` and `target` must be of the same length. The content of both arrays' object(s) depends on the given `phemeType`.
	
	{	
		target: [{}, ...],
		prediction: [{}, ...]
	}
	

#### Mass Spectra










