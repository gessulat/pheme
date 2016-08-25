#Pheme
With Pheme you can compare predictions against some ground truth visually. Visualizations are specific to the data type of the prediction. Currently available data types are:

- mass spectra


![screenshot](images/pheme.jpg =650x)

---
# Installation

You need to install:

- Node + npm
- polymer-cli with `npm install -g polymer-cli`

Then run `polymer serve -o` in the project's root directory.

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










