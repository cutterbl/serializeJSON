# **serializeJSON** 0.0.2

MIT License

jQuery plugin that wraps jQuery's serializeArray() output, and maps the key values as a single object, 
including turning multiple fields of the same name into a list of values with a single key. Plugin does
no type checking/conversion. It just pulls the data together into a neat object. Perfect for 'POST' data.

#**Usage**

    var formData = $(someForm).serializeJSON();
    $.ajax({
        url: '/some/endpoint',
        method: 'POST',
        data: formData
    });
