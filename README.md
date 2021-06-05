# Validation
using: 
	Validator({
		form: name-form,
		formGroupSelector: name-form-group,
		selectorMessage: name-form-message-error,
		rules: [
			Validator.isRequired(selector, message),
			Validator.isEmail(selector, message),
			Validator.minLenth(selector, min, message),
			Validator.ref(selector, function() => valueConfirm),
		],
		onSubmit: (data) => {
			// Call API
		}
	})
