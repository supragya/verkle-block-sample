# Example of a block root with a Verkle state root

## Block content

This is a standard RLP block containing 3 transactions, and an added `VerkleProof` field at the end of the block header.

```
> rlpdump block2.rlp
[
  # Block Header
  [
    2a0fa77c9673bac5696974f6693b917bd391bcbfe564e1d246ebaa9835255c8a,
    1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347,
    0000000000000000000000000000000000000000,
    03aec4276033869b5900313c7d807cdaa948e38acd9aa43c98e05089adc7389d,
    145d1893587d0bcae212d39729190212236500e5c441a269f980381c611bebac,
    251fdcdd3e713f5799e22aaec5341cdc5874392a80e89b2f70766a83806f77d4,
    00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000,
    020000,
    02,       # Block number
    47e7c4,
    018768,
    14,
    "",
    0000000000000000000000000000000000000000000000000000000000000000,
    0000000000000000,
    2de97bd1,
    
    # Serialized proof
000000000f0000000a0a0a0a0a0a0a0a0a0a0a0a0a0a0a06000000ec6d205b6beff33c492e18fc08c94b94ed386456e00314ace17cc7f9ee42d5e39755fbb89595223c3e690fa145b6023b7fd09d928612f5ac11c580186b836607e003fbe47c395bc02d30927ed826c39b1709e6724d1e4129afd8b933ecdbb9dfd0ada94181e64bd9a25bfb5bd12995e0cf21805857eb62ee9dbf7757f2fef094ba361b815bf0ad5910cb6233f939edc0b64be8e480612ed753b7fb37868c5e9c44aa8422b47acb0e388e8c33391c5898f9082c86b539e652cbe30f177d3d1018dac702b22ae7d7c4549c03f9812281ea8126b03f58e5ba4ee0a90b0748d215386dad3d3b3faef1955face09fc6e2941e4a803eaab01393399bccb18bc4abcc546b77e81678c6104d6ef22a9e945f98640598fbb09f90864c899fb34f2b48e1698b57e7f3eabab4b1bf7fdaa6a22786964b89e982ec584d4aa84b02c0e6c15f1ffa5d1425cb40cf440729c66cfd81ba7c7dc680a29f87b97098819daf898bb13c251229824e34ed19a5c70407a16a59d44057628e7eb5d560444c68135c3e5a9ae5997ea21f5c699ef0c6371eb0956406bf8c3de0eae26e5061c71db9151e092ad2765825c7c866d128f34aa21473e11e4be395a86f6b3a84ff08799cedee2fd410e7afc83776d04da6d8134d0b8c7e2ccab7e7cdb2dce3bf78ac30bd5591c3a2277b59ecc79bd30d4cd6c9db3a5a15cf95bf5a1060cd2c2b43d9410b2a2cce448bc39c756bd029ac9cbe4f4664efbb450b71f12e0202252e96afb304c115d50fd33bbbcdc13f050d151ed0d276f41219252a4971d007a81ac327fdbb2340d5b9cbdf46be86a2a3c9454e28dcc9f88a4b2648a2e9f1d7902b7744ebea12d5dc3f3887877f86cdb5139701b5f50e53297b1bf86d8c7e0eefc385db4b81d6749198babf82141f5551b7376e808915f8bcd9da97f0084d9b5fff1e373fb1b625f84222e64cded4d063e67ed0b3704df62fb3fe81314f6835a09a49446999928044de343977a7235dc921d47fd235acb90d842e38751a4eee1a9f25aa026b90427d152d1ddfc0fcaf58d52dac6ae360442023c2785e411cf5b2b795c9b96aea2d8b06,

    # List of (key, values) of the pre-state, that are accessed during the
    # block's execution.
    [
      [
        318dea512b6f3237a2d4763cf49bf26de3b617fb0cabe38a97807a5549df4d01,
        320122e8584be00d,
      ],
      [
        e6ed6c222e3985050b4fc574b136b0a42c63538e9ab970995cd418ba8e526400,
        0000000000000000000000000000000000000000000000000000000000000000,
      ],
      [
        318dea512b6f3237a2d4763cf49bf26de3b617fb0cabe38a97807a5549df4d03,
        "",
      ],
      [
        18fb432d3b859ec3a1803854e8cceea75d092e52d0d4a4398d13022496745a02,
        0000000000000000,
      ],
      [
        318dea512b6f3237a2d4763cf49bf26de3b617fb0cabe38a97807a5549df4d02,
        0300000000000000,
      ],
      [
        18fb432d3b859ec3a1803854e8cceea75d092e52d0d4a4398d13022496745a04,
        0000000000000000000000000000000000000000000000000000000000000000,
      ],
      [
        e6ed6c222e3985050b4fc574b136b0a42c63538e9ab970995cd418ba8e526402,
        0000000000000000,
      ],
      [
        e6ed6c222e3985050b4fc574b136b0a42c63538e9ab970995cd418ba8e526403,
        c5d2460186f7233c927e7db2dcc703c0e500b653ca82273b7bfad8045d85a470,
      ],
      [
        318dea512b6f3237a2d4763cf49bf26de3b617fb0cabe38a97807a5549df4d04,
        "",
      ],
      [
        18fb432d3b859ec3a1803854e8cceea75d092e52d0d4a4398d13022496745a00,
        0000000000000000000000000000000000000000000000000000000000000000,
      ],
      [
        18fb432d3b859ec3a1803854e8cceea75d092e52d0d4a4398d13022496745a03,
        c5d2460186f7233c927e7db2dcc703c0e500b653ca82273b7bfad8045d85a470,
      ],
      [
        e6ed6c222e3985050b4fc574b136b0a42c63538e9ab970995cd418ba8e526401,
        1bc176f2790c91e6,
      ],
      [
        e6ed6c222e3985050b4fc574b136b0a42c63538e9ab970995cd418ba8e526404,
        0000000000000000000000000000000000000000000000000000000000000000,
      ],
      [
        318dea512b6f3237a2d4763cf49bf26de3b617fb0cabe38a97807a5549df4d00,
        0000000000000000000000000000000000000000000000000000000000000000,
      ],
      [
        18fb432d3b859ec3a1803854e8cceea75d092e52d0d4a4398d13022496745a01,
        e703,
      ],
    ],
  ],
  
  # Transaction list
  [
    [
      03,
      342770c0,
      878c,
      0102030000000000000000000000000000000000,
      03e7,
      "",
      "&",
      b5052005e25c9c5f8100a37d9aad8c3057969170cb239b03b7615c5619b73979,
      50d23a8e2796503706568c13de56d45a232903b84f55a5c663383988fb559642,
    ],
    [
      04,
      342770c0,
      878c,
      0000000000000000000000000000000000000000,
      03e7,
      "",
      "%",
      f8ea4ce9a209cf2feee581a3a5e263bd48d0732c77ae9c723f7ec0a18ac16dd8,
      6f0e4bd905d8acbb6273fd6bed78548e9544bf48634d86234715b4f92bf89bfe,
    ],
    [
      05,
      342770c0,
      "xP",
      0000000000000000000000000000000000000000,
      "",
      "",
      "%",
      37d860df9bfdcdedc84ad76dc2281c330f925b02eeff90b63162067b33abae07,
      7d0f5b4341b449320c59529a44ac98582c7957611b723f1fc686b8a3801d88bf,
    ],
  ],
  [],
]

```

## Verkle proof format

This section is subject to change, so make sure that you watch this description as it will be udpated.

The verkle tree update adds two extra fields for the block: a proof and a list of (key, values) representing the _pre_ state of a block.

| Field | Block Header index | Description | Format |
| ----- | :----------------: | ----------- | ------ |
| Proof | 16 | Binary payload to pass to `rust-verkle` directly:<br /> * len(Proof of absence stem) ++ Proof of absence stems <br /> * len(depths) ++ serialize(depthi ++ ext statusi) <br /> * len(commitments) ++ serialize(commitment)<br /> * Multipoint proof | Flat binary
| Key, values | 17 | For each (key, value): a list of two byte arrays. The first array is the 32-byte key, and the second array is a 32-byte value (if present) or an empty array (if absent) | RLP |

## Changelog

  * 22.01.22 - Initial version
  * 27.01.22:
    * proof and key,values lists are embedded in two distinct fields of the block (indices 16 and 17, respectively)
    * fix a duplicaiton issue for the commitments
    * remove the root commitment from the list
    * sort commitments by path
  * 28.01.22:
    * the keys and values are now encoded in the block with RLP

## TODO

 * [x] RLP encoding of the structure encapsulating the proof and the (key, values) tuples
 * [ ] SSZ encoding of that same structure when the final format has been defined
