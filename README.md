# @megafon/msisdn

[![npm (scoped with tag)](https://img.shields.io/npm/v/@megafon/msisdn/latest?label=%40megafon%2Fmsisdn)](https://www.npmjs.com/package/@megafon/msisdn/v/latest) 
[![Github Actions](https://github.com/MegafonWebLab/msisdn/workflows/msisdn%20CI/badge.svg)](https://github.com/MegafonWebLab/msisdn/actions)

Russian msisdn normalizer and formatter.

## Installation

```
$ yarn add @megafon/msisdn
```

## Usage

# change

```typescript
import { clean, pretty, PrettyFormats } from '@megafon/msisdn';

const userNumber = '+7 926 000-00-00';

console.log(clean(userNumber)); // Prints: '9260000000'
console.log(pretty(userNumber, PrettyFormats.ZETA)); // Prints: '+7 (926) 000-00-00'
```

### Available formats:

* alpha: 9161234567
* beta: 79161234567
* gamma: 916 123-4567
* delta: (916) 123-4567
* epsilon: +7 (916) 123-4567
* zeta: +7 (916) 123-45-67

## Contributing

Follow [CONTRIBUTING.md](CONTRIBUTING.md) and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).
