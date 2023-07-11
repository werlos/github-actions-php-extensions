### GitHub Actions with/without "none" in PHP extensions

| OS      | Extensions config              | #  |  curl? | opcache? | mbstring? | bcmath?
|---------|--------------------------------|----|--------|----------|-----------|--------
| Ubuntu  | curl, opcache, :mbstring       | 89 |  yes   | yes      | no        | yes
| Ubuntu  | none, curl, opcache, :mbstring | 24 |  yes   | yes      | no        | no
| Windows | curl, opcache, :mbstring       | 35 |  yes   | yes      | no        | yes
| Windows | none, curl, opcache, :mbstring | 34 |  yes   | yes      | no        | yes
| macOS   | curl, opcache, :mbstring       | 69 |  yes   | yes      | yes       | yes
| macOS   | none, curl, opcache, :mbstring | 67 |  yes   | no       | yes       | yes

`#` is result of `php -m | wc -l`
