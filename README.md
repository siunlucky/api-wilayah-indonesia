## ENDPOINTS

#### 1. Mengambil Daftar Provinsi

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/provinces.json
```

Contoh Response:

```
[
  {
    "id": "11",
    "name": "ACEH"
  },
  {
    "id": "12",
    "name": "SUMATERA UTARA"
  },
  ...
]
```

#### 2. Mengambil Daftar Kab/Kota pada Provinsi Tertentu

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/regencies/{provinceId}.json
```

Contoh untuk mengambil daftar kab/kota di provinsi Aceh (ID = 11):

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/regencies/11.json
```

Contoh Response:

```
[
  {
    "id": "1101",
    "province_id": "11",
    "name": "KABUPATEN SIMEULUE"
  },
  {
    "id": "1102",
    "province_id": "11",
    "name": "KABUPATEN ACEH SINGKIL"
  },
  ...
]
```

#### 3. Mengambil Daftar Kecamatan pada Kab/Kota Tertentu

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/districts/{regencyId}.json
```

Contoh untuk mengambil daftar kecamatan di Aceh Selatan (ID = 1103):

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/districts/1103.json
```

Contoh Response:

```
[
  {
    "id": "1103010",
    "regency_id": "1103",
    "name": "TRUMON"
  },
  {
    "id": "1103011",
    "regency_id": "1103",
    "name": "TRUMON TIMUR"
  },
  ...
]
```

#### 4. Mengambil Daftar Kelurahan pada Kecamatan Tertentu

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/villages/{districtId}.json
```

Contoh untuk mengambil daftar kelurahan di Trumon (ID = 1103010):

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/villages/1103010.json
```

Contoh Response:

```
[
  {
    "id": "1103010001",
    "district_id": "1103010",
    "name": "KUTA PADANG"
  },
  {
    "id": "1103010002",
    "district_id": "1103010",
    "name": "RAKET"
  },
  ...
]
```

#### 5. Mengambil Data Provinsi berdasarkan ID Provinsi

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/province/{provinceId}.json
```

Contoh untuk mengambil data provinsi Aceh (ID = 11):

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/province/11.json
```

Contoh Response:

```
{
  "id": "11",
  "name": "ACEH"
}
```

#### 6. Mengambil Data Kab/Kota berdasarkan ID Kab/Kota

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/regency/{regencyId}.json
```

Contoh untuk mengambil data kabupaten Aceh Selatan (ID = 1103):

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/regency/1103.json
```

Contoh Response:

```
{
  "id": "1103",
  "province_id": "11",
  "name": "KABUPATEN ACEH SELATAN"
}
```

#### 7. Mengambil Data Kecamatan berdasarkan ID Kecamatan

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/district/{districtId}.json
```

Contoh untuk mengambil data kecamatan Trumon Timur (ID = 1103011):

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/district/1103011.json
```

Contoh Response:

```
{
  "id": "1103011",
  "regency_id": "1103",
  "name": "TRUMON TIMUR"
}
```

#### 8. Mengambil Data Kelurahan berdasarkan ID Kelurahan

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/village/{villageId}.json
```

Contoh untuk mengambil data kelurahan Jambo Dalem (ID = 1103011010):

```
GET https://siunlucky.github.io/api-wilayah-indonesia/api/village/1103011010.json
```

Contoh Response:

```
{
  "id": "1103011010",
  "district_id": "1103011",
  "name": "JAMBO DALEM"
}
```
