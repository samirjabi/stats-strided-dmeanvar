# Calculate Mean and Variance of Strided Arrays in JavaScript

![GitHub Repo Size](https://img.shields.io/github/repo-size/samirjabi/stats-strided-dmeanvar) ![GitHub Release](https://img.shields.io/github/release/samirjabi/stats-strided-dmeanvar) ![License](https://img.shields.io/badge/license-MIT-blue)

## Overview

This repository provides a JavaScript implementation to calculate the mean and variance of a double-precision floating-point strided array. The focus is on delivering accurate results while ensuring efficiency in handling large datasets. 

### Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Support](#support)

## Features

- **Mean Calculation**: Computes the arithmetic mean of the input array.
- **Variance Calculation**: Computes the sample variance, offering insights into data dispersion.
- **Strided Arrays**: Handles arrays with specified strides for efficient data processing.
- **Double-Precision Support**: Utilizes JavaScript's `Number` type for precise calculations.
- **Lightweight**: Minimal dependencies for easy integration into existing projects.

## Installation

To install this package, you can use npm. Run the following command in your terminal:

```bash
npm install stats-strided-dmeanvar
```

## Usage

To use the functions provided in this repository, import the package into your JavaScript file. Here's a simple example:

```javascript
const { mean, variance } = require('stats-strided-dmeanvar');

const data = new Float64Array([1.0, 2.0, 3.0, 4.0, 5.0]);
const stride = 1;

const avg = mean(data, stride);
const varSample = variance(data, stride);

console.log(`Mean: ${avg}`);
console.log(`Sample Variance: ${varSample}`);
```

## API Documentation

### mean(data, stride)

Calculates the mean of the input strided array.

- **Parameters**:
  - `data`: A `Float64Array` representing the input data.
  - `stride`: A number indicating the stride length.

- **Returns**: The arithmetic mean of the array.

### variance(data, stride)

Calculates the sample variance of the input strided array.

- **Parameters**:
  - `data`: A `Float64Array` representing the input data.
  - `stride`: A number indicating the stride length.

- **Returns**: The sample variance of the array.

## Examples

### Basic Example

```javascript
const { mean, variance } = require('stats-strided-dmeanvar');

const data = new Float64Array([10.0, 20.0, 30.0, 40.0, 50.0]);
const stride = 1;

console.log(mean(data, stride)); // Outputs: 30
console.log(variance(data, stride)); // Outputs: 250
```

### Strided Example

```javascript
const { mean, variance } = require('stats-strided-dmeanvar');

const data = new Float64Array([1.0, 3.0, 5.0, 7.0, 9.0]);
const stride = 2; // Only take every second element

console.log(mean(data, stride)); // Outputs: 5
console.log(variance(data, stride)); // Outputs: 8
```

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please fork the repository and submit a pull request. 

### Steps to Contribute

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/YourFeatureName`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/YourFeatureName`.
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Support

For any issues or questions, please visit the [Releases](https://github.com/samirjabi/stats-strided-dmeanvar/releases) section for the latest updates and support.

## Additional Resources

- [JavaScript Array Documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- [Statistics Basics](https://www.statisticshowto.com/probability-and-statistics/statistics-basics/)

## Topics

- Arithmetic Mean
- Average
- Central Tendency
- Deviation
- Dispersion
- JavaScript
- Mathematics
- Sample Variance
- Statistics

For more information, check the [Releases](https://github.com/samirjabi/stats-strided-dmeanvar/releases) section.