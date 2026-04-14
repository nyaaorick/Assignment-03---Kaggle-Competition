6.3s 1 0.00s - Debugger warning: It seems that frozen modules are being used, which may
6.3s 2 0.00s - make the debugger miss breakpoints. Please pass -Xfrozen_modules=off
6.3s 3 0.00s - to python to disable frozen modules.
6.3s 4 0.00s - Note: Debugging will proceed. Set PYDEVD_DISABLE_FILE_VALIDATION=1 to disable this validation.
7.0s 5 0.00s - Debugger warning: It seems that frozen modules are being used, which may
7.0s 6 0.00s - make the debugger miss breakpoints. Please pass -Xfrozen_modules=off
7.0s 7 0.00s - to python to disable frozen modules.
7.0s 8 0.00s - Note: Debugging will proceed. Set PYDEVD_DISABLE_FILE_VALIDATION=1 to disable this validation.
28.0s 9 Torch: 2.10.0+cu128
28.0s 10 CUDA available: True
28.0s 11 timm: 1.0.25
28.0s 12 torchvision: 0.25.0+cu128
28.0s 13 Iterative stratification ready
28.1s 14 Train dir: /kaggle/input/competitions/plant-pathology-2021-fgvc8/train_images
28.1s 15 Test dir : /kaggle/input/competitions/plant-pathology-2021-fgvc8/test_images
28.1s 16 Device   : cuda
28.1s 17 Num GPUs : 2
28.1s 18 In notebook: True
28.1s 19 Use DDP  : False
28.1s 20 Use DataParallel: True
28.1s 21 World size: 1
28.1s 22 Num folds: 3
28.1s 23 Selected folds: [0]
28.1s 24 Train batch size (global): 32
28.1s 25 Eval image batch size: 32
28.1s 26 Tile inference batch size: 8
28.1s 27 Training uses local crops with scale: (0.5, 1.0)
28.1s 28 Train CPU max long edge: 2048
28.1s 29 RandAug enabled: True
28.1s 30 RandAug ops/magnitude: (2, 7)
28.1s 31 Inference tiling enabled: True
28.1s 32 Configured workers: 2
28.1s 33 Active DataLoader workers: 0
28.1s 34 Train shape: (18632, 2)
28.1s 35 Sample submission shape: (3, 2)
28.1s 36 
28.1s 37 First 5 rows:
28.1s 38 image                           labels
28.1s 39 0  800113bb65efe69e.jpg                          healthy
28.1s 40 1  8002cb321f8bfcdf.jpg  scab frog_eye_leaf_spot complex
28.1s 41 2  80070f7fb5e2ccaa.jpg                             scab
28.1s 42 3  80077517781fb94f.jpg                             scab
28.1s 43 4  800cbf0ff87721f8.jpg                          complex
28.1s 44 
28.1s 45 Classes: ['complex', 'frog_eye_leaf_spot', 'healthy', 'powdery_mildew', 'rust', 'scab']
28.2s 46 Most common label strings:
28.2s 47 labels
28.2s 48 scab                               4826
28.2s 49 healthy                            4624
28.2s 50 frog_eye_leaf_spot                 3181
28.2s 51 rust                               1860
28.2s 52 complex                            1602
28.2s 53 powdery_mildew                     1184
28.2s 54 scab frog_eye_leaf_spot             686
28.2s 55 scab frog_eye_leaf_spot complex     200
28.2s 56 frog_eye_leaf_spot complex          165
28.2s 57 rust frog_eye_leaf_spot             120
28.2s 58 rust complex                         97
28.2s 59 powdery_mildew complex               87
28.2s 60 Name: count, dtype: int64
31.8s 61 Label matrix shape: (18632, 6)
31.8s 62 
31.8s 63 Overall per-class positive rate:
31.8s 64 scab                  0.306569
31.8s 65 healthy               0.248175
31.8s 66 frog_eye_leaf_spot    0.233577
31.8s 67 complex               0.115447
31.8s 68 rust                  0.111475
31.8s 69 powdery_mildew        0.068216
31.8s 70 dtype: float32
31.8s 71 
31.8s 72 Test images: 3
31.8s 73 
31.8s 74 Fold sizes:
31.8s 75 fold  train_size  val_size
31.8s 76 0     0       12447      6185
31.8s 77 1     1       12392      6240
31.8s 78 2     2       12425      6207
31.8s 79 
31.8s 80 Per-class validation positive rate by fold:
31.8s 81 overall_positive_rate  fold_0_val_rate  fold_1_val_rate  \
31.8s 82 complex                            0.1154           0.1159           0.1149
31.8s 83 frog_eye_leaf_spot                 0.2336           0.2346           0.2324
31.8s 84 healthy                            0.2482           0.2492           0.2470
31.8s 85 powdery_mildew                     0.0682           0.0686           0.0678
31.8s 86 rust                               0.1115           0.1119           0.1111
31.8s 87 scab                               0.3066           0.3078           0.3051
31.8s 88 
31.8s 89 fold_2_val_rate
31.8s 90 complex                      0.1155
31.8s 91 frog_eye_leaf_spot           0.2338
31.8s 92 healthy                      0.2484
31.8s 93 powdery_mildew               0.0683
31.8s 94 rust                         0.1115
31.8s 95 scab                         0.3068
44.1s 96 Selected timm model: vit_small_patch14_dinov2.lvd142m
44.1s 97 Normalization mean: (0.485, 0.456, 0.406)
44.1s 98 Normalization std : (0.229, 0.224, 0.225)
44.1s 99 Preview fold      : 0
44.1s 100 Train batch image count: 32
44.1s 101 First raw train image tensor shape: (3, 1536, 2048)
44.1s 102 First raw train image tensor dtype: torch.uint8
44.1s 103 First augmented train image tensor shape: (3, 518, 518)
44.1s 104 First augmented train image tensor dtype: torch.float32
44.1s 105 Train batch target tensor shape: (32, 6)
45.5s 106 Validation full-image batch size: 8
45.5s 107 First full image tensor shape: (3, 2672, 4000)
45.5s 108 First full image tensor dtype: torch.uint8
45.5s 109 Validation target tensor shape: (8, 6)
45.5s 110 Example image name: 80077517781fb94f.jpg
46.3s 111 PlantDiseaseDINOv2Model(
46.3s 112 (backbone): VisionTransformer(
46.3s 113 (patch_embed): PatchEmbed(
46.3s 114 (proj): Conv2d(3, 384, kernel_size=(14, 14), stride=(14, 14))
46.3s 115 (norm): Identity()
46.3s 116 )
46.3s 117 (pos_drop): Dropout(p=0.0, inplace=False)
46.3s 118 (patch_drop): Identity()
46.3s 119 (norm_pre): Identity()
46.3s 120 (blocks): Sequential(
46.3s 121 (0): Block(
46.3s 122 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 123 (attn): Attention(
46.3s 124 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 125 (q_norm): Identity()
46.3s 126 (k_norm): Identity()
46.3s 127 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 128 (norm): Identity()
46.3s 129 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 130 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 131 )
46.3s 132 (ls1): LayerScale()
46.3s 133 (drop_path1): Identity()
46.3s 134 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 135 (mlp): Mlp(
46.3s 136 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 137 (act): GELU(approximate='none')
46.3s 138 (drop1): Dropout(p=0.0, inplace=False)
46.3s 139 (norm): Identity()
46.3s 140 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 141 (drop2): Dropout(p=0.0, inplace=False)
46.3s 142 )
46.3s 143 (ls2): LayerScale()
46.3s 144 (drop_path2): Identity()
46.3s 145 )
46.3s 146 (1): Block(
46.3s 147 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 148 (attn): Attention(
46.3s 149 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 150 (q_norm): Identity()
46.3s 151 (k_norm): Identity()
46.3s 152 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 153 (norm): Identity()
46.3s 154 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 155 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 156 )
46.3s 157 (ls1): LayerScale()
46.3s 158 (drop_path1): Identity()
46.3s 159 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 160 (mlp): Mlp(
46.3s 161 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 162 (act): GELU(approximate='none')
46.3s 163 (drop1): Dropout(p=0.0, inplace=False)
46.3s 164 (norm): Identity()
46.3s 165 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 166 (drop2): Dropout(p=0.0, inplace=False)
46.3s 167 )
46.3s 168 (ls2): LayerScale()
46.3s 169 (drop_path2): Identity()
46.3s 170 )
46.3s 171 (2): Block(
46.3s 172 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 173 (attn): Attention(
46.3s 174 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 175 (q_norm): Identity()
46.3s 176 (k_norm): Identity()
46.3s 177 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 178 (norm): Identity()
46.3s 179 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 180 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 181 )
46.3s 182 (ls1): LayerScale()
46.3s 183 (drop_path1): Identity()
46.3s 184 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 185 (mlp): Mlp(
46.3s 186 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 187 (act): GELU(approximate='none')
46.3s 188 (drop1): Dropout(p=0.0, inplace=False)
46.3s 189 (norm): Identity()
46.3s 190 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 191 (drop2): Dropout(p=0.0, inplace=False)
46.3s 192 )
46.3s 193 (ls2): LayerScale()
46.3s 194 (drop_path2): Identity()
46.3s 195 )
46.3s 196 (3): Block(
46.3s 197 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 198 (attn): Attention(
46.3s 199 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 200 (q_norm): Identity()
46.3s 201 (k_norm): Identity()
46.3s 202 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 203 (norm): Identity()
46.3s 204 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 205 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 206 )
46.3s 207 (ls1): LayerScale()
46.3s 208 (drop_path1): Identity()
46.3s 209 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 210 (mlp): Mlp(
46.3s 211 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 212 (act): GELU(approximate='none')
46.3s 213 (drop1): Dropout(p=0.0, inplace=False)
46.3s 214 (norm): Identity()
46.3s 215 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 216 (drop2): Dropout(p=0.0, inplace=False)
46.3s 217 )
46.3s 218 (ls2): LayerScale()
46.3s 219 (drop_path2): Identity()
46.3s 220 )
46.3s 221 (4): Block(
46.3s 222 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 223 (attn): Attention(
46.3s 224 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 225 (q_norm): Identity()
46.3s 226 (k_norm): Identity()
46.3s 227 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 228 (norm): Identity()
46.3s 229 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 230 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 231 )
46.3s 232 (ls1): LayerScale()
46.3s 233 (drop_path1): Identity()
46.3s 234 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 235 (mlp): Mlp(
46.3s 236 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 237 (act): GELU(approximate='none')
46.3s 238 (drop1): Dropout(p=0.0, inplace=False)
46.3s 239 (norm): Identity()
46.3s 240 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 241 (drop2): Dropout(p=0.0, inplace=False)
46.3s 242 )
46.3s 243 (ls2): LayerScale()
46.3s 244 (drop_path2): Identity()
46.3s 245 )
46.3s 246 (5): Block(
46.3s 247 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 248 (attn): Attention(
46.3s 249 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 250 (q_norm): Identity()
46.3s 251 (k_norm): Identity()
46.3s 252 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 253 (norm): Identity()
46.3s 254 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 255 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 256 )
46.3s 257 (ls1): LayerScale()
46.3s 258 (drop_path1): Identity()
46.3s 259 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 260 (mlp): Mlp(
46.3s 261 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 262 (act): GELU(approximate='none')
46.3s 263 (drop1): Dropout(p=0.0, inplace=False)
46.3s 264 (norm): Identity()
46.3s 265 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 266 (drop2): Dropout(p=0.0, inplace=False)
46.3s 267 )
46.3s 268 (ls2): LayerScale()
46.3s 269 (drop_path2): Identity()
46.3s 270 )
46.3s 271 (6): Block(
46.3s 272 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 273 (attn): Attention(
46.3s 274 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 275 (q_norm): Identity()
46.3s 276 (k_norm): Identity()
46.3s 277 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 278 (norm): Identity()
46.3s 279 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 280 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 281 )
46.3s 282 (ls1): LayerScale()
46.3s 283 (drop_path1): Identity()
46.3s 284 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 285 (mlp): Mlp(
46.3s 286 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 287 (act): GELU(approximate='none')
46.3s 288 (drop1): Dropout(p=0.0, inplace=False)
46.3s 289 (norm): Identity()
46.3s 290 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 291 (drop2): Dropout(p=0.0, inplace=False)
46.3s 292 )
46.3s 293 (ls2): LayerScale()
46.3s 294 (drop_path2): Identity()
46.3s 295 )
46.3s 296 (7): Block(
46.3s 297 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 298 (attn): Attention(
46.3s 299 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 300 (q_norm): Identity()
46.3s 301 (k_norm): Identity()
46.3s 302 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 303 (norm): Identity()
46.3s 304 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 305 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 306 )
46.3s 307 (ls1): LayerScale()
46.3s 308 (drop_path1): Identity()
46.3s 309 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 310 (mlp): Mlp(
46.3s 311 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 312 (act): GELU(approximate='none')
46.3s 313 (drop1): Dropout(p=0.0, inplace=False)
46.3s 314 (norm): Identity()
46.3s 315 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 316 (drop2): Dropout(p=0.0, inplace=False)
46.3s 317 )
46.3s 318 (ls2): LayerScale()
46.3s 319 (drop_path2): Identity()
46.3s 320 )
46.3s 321 (8): Block(
46.3s 322 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 323 (attn): Attention(
46.3s 324 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 325 (q_norm): Identity()
46.3s 326 (k_norm): Identity()
46.3s 327 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 328 (norm): Identity()
46.3s 329 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 330 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 331 )
46.3s 332 (ls1): LayerScale()
46.3s 333 (drop_path1): Identity()
46.3s 334 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 335 (mlp): Mlp(
46.3s 336 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 337 (act): GELU(approximate='none')
46.3s 338 (drop1): Dropout(p=0.0, inplace=False)
46.3s 339 (norm): Identity()
46.3s 340 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 341 (drop2): Dropout(p=0.0, inplace=False)
46.3s 342 )
46.3s 343 (ls2): LayerScale()
46.3s 344 (drop_path2): Identity()
46.3s 345 )
46.3s 346 (9): Block(
46.3s 347 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 348 (attn): Attention(
46.3s 349 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 350 (q_norm): Identity()
46.3s 351 (k_norm): Identity()
46.3s 352 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 353 (norm): Identity()
46.3s 354 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 355 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 356 )
46.3s 357 (ls1): LayerScale()
46.3s 358 (drop_path1): Identity()
46.3s 359 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 360 (mlp): Mlp(
46.3s 361 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 362 (act): GELU(approximate='none')
46.3s 363 (drop1): Dropout(p=0.0, inplace=False)
46.3s 364 (norm): Identity()
46.3s 365 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 366 (drop2): Dropout(p=0.0, inplace=False)
46.3s 367 )
46.3s 368 (ls2): LayerScale()
46.3s 369 (drop_path2): Identity()
46.3s 370 )
46.3s 371 (10): Block(
46.3s 372 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 373 (attn): Attention(
46.3s 374 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 375 (q_norm): Identity()
46.3s 376 (k_norm): Identity()
46.3s 377 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 378 (norm): Identity()
46.3s 379 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 380 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 381 )
46.3s 382 (ls1): LayerScale()
46.3s 383 (drop_path1): Identity()
46.3s 384 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 385 (mlp): Mlp(
46.3s 386 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 387 (act): GELU(approximate='none')
46.3s 388 (drop1): Dropout(p=0.0, inplace=False)
46.3s 389 (norm): Identity()
46.3s 390 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 391 (drop2): Dropout(p=0.0, inplace=False)
46.3s 392 )
46.3s 393 (ls2): LayerScale()
46.3s 394 (drop_path2): Identity()
46.3s 395 )
46.3s 396 (11): Block(
46.3s 397 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 398 (attn): Attention(
46.3s 399 (qkv): Linear(in_features=384, out_features=1152, bias=True)
46.3s 400 (q_norm): Identity()
46.3s 401 (k_norm): Identity()
46.3s 402 (attn_drop): Dropout(p=0.0, inplace=False)
46.3s 403 (norm): Identity()
46.3s 404 (proj): Linear(in_features=384, out_features=384, bias=True)
46.3s 405 (proj_drop): Dropout(p=0.0, inplace=False)
46.3s 406 )
46.3s 407 (ls1): LayerScale()
46.3s 408 (drop_path1): Identity()
46.3s 409 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 410 (mlp): Mlp(
46.3s 411 (fc1): Linear(in_features=384, out_features=1536, bias=True)
46.3s 412 (act): GELU(approximate='none')
46.3s 413 (drop1): Dropout(p=0.0, inplace=False)
46.3s 414 (norm): Identity()
46.3s 415 (fc2): Linear(in_features=1536, out_features=384, bias=True)
46.3s 416 (drop2): Dropout(p=0.0, inplace=False)
46.3s 417 )
46.3s 418 (ls2): LayerScale()
46.3s 419 (drop_path2): Identity()
46.3s 420 )
46.3s 421 )
46.3s 422 (norm): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
46.3s 423 (fc_norm): Identity()
46.3s 424 (head_drop): Dropout(p=0.0, inplace=False)
46.3s 425 (head): Identity()
46.3s 426 )
46.3s 427 (head): Sequential(
46.3s 428 (0): LayerNorm((384,), eps=1e-05, elementwise_affine=True)
46.3s 429 (1): Dropout(p=0.3, inplace=False)
46.3s 430 (2): Linear(in_features=384, out_features=256, bias=True)
46.3s 431 (3): GELU(approximate='none')
46.3s 432 (4): Dropout(p=0.2, inplace=False)
46.3s 433 (5): Linear(in_features=256, out_features=6, bias=True)
46.3s 434 )
46.3s 435 )
46.3s 436 
46.3s 437 Trainable parameters after freezing backbone: 100870
47.0s 438 
47.0s 439 ============ Running Selected Fold 0 ============
47.0s 440 Checkpoint path: /kaggle/working/best_dinov2_small_plant_pathology_fold0.pth
47.0s 441 Distributed training: False
47.0s 442 DataParallel training: True
47.0s 443 Global train batch size: 32
47.0s 444 Tile inference batch size: 8
47.0s 445 Trainable parameters after freezing backbone: 100870
4923.3s 446 Head training | Epoch 01/3 | train_loss=0.2544 | train_f1=0.6580 | val_image_f1=0.7648 | val_default_f1=0.7078 | val_agg=mean
9829.8s 447 Head training | Epoch 02/3 | train_loss=0.2059 | train_f1=0.7372 | val_image_f1=0.7971 | val_default_f1=0.6949 | val_agg=mean
14512.7s 448 Head training | Epoch 03/3 | train_loss=0.1939 | train_f1=0.7570 | val_image_f1=0.8079 | val_default_f1=0.7276 | val_agg=mean
14512.8s 449 Reloaded best checkpoint from stage: Head training (val_f1=0.8079, agg=mean)
14512.8s 450 Trainable parameters after partial unfreeze: 3652102
14512.8s 451 Backbone parameter groups: 30
14512.8s 452 Head parameter groups    : 6
19302.5s 453 Fine-tuning | Epoch 01/3 | train_loss=0.1438 | train_f1=0.8199 | val_image_f1=0.8480 | val_default_f1=0.7966 | val_agg=mean
24011.7s 454 Fine-tuning | Epoch 02/3 | train_loss=0.1158 | train_f1=0.8581 | val_image_f1=0.8638 | val_default_f1=0.8177 | val_agg=mean
28753.9s 455 Fine-tuning | Epoch 03/3 | train_loss=0.1056 | train_f1=0.8722 | val_image_f1=0.8636 | val_default_f1=0.8402 | val_agg=mean
28753.9s 456 Reloaded best checkpoint from stage: Fine-tuning (val_f1=0.8638, agg=mean)
30573.0s 457 Selected fold run finished.
30573.0s 458 
30573.0s 459 Per-selected-fold summary:
30573.0s 460 fold  train_size  val_size   best_stage  best_epoch selected_method  \
30573.0s 461 0     0       12447      6185  Fine-tuning           2            mean
30573.0s 462 
30573.0s 463 best_val_f1                                    checkpoint_path
30573.0s 464 0     0.863753  /kaggle/working/best_dinov2_small_plant_pathol...
30573.0s 465 
30573.0s 466 Aggregation summary across selected folds:
30573.0s 467 aggregation_method  mean_default_f1  mean_tuned_f1  std_tuned_f1
30573.0s 468 0               mean           0.8177         0.8638           0.0
30573.0s 469 1                max           0.7733         0.7915           0.0
30573.1s 470 Aggregation summary across selected folds:
30573.1s 471 aggregation_method  mean_default_f1  mean_tuned_f1  std_tuned_f1
30573.1s 472 0               mean           0.8177         0.8638           0.0
30573.1s 473 1                max           0.7733         0.7915           0.0
30573.1s 474 
30573.1s 475 Selected aggregation method by selected-fold mean tuned F1: mean
30573.1s 476 Mean tuned F1: 0.8638 +/- 0.0000
30573.1s 477 Single-model submission fold: 0
30573.1s 478 Thresholds used for the submission fold:
30573.1s 479 complex: 0.30
30573.1s 480 frog_eye_leaf_spot: 0.30
30573.1s 481 healthy: 0.60
30573.1s 482 powdery_mildew: 0.50
30573.1s 483 rust: 0.20
30573.1s 484 scab: 0.40
30573.6s 485 Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
30573.6s 486 
30573.6s 487 Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
30574.4s 488 Submission fold: 0
30574.4s 489 Checkpoint stage: Fine-tuning
30574.4s 490 Aggregation used: mean
30574.4s 491 
30574.4s 492 Sample predictions:
30574.4s 493 85f8cb619c66b863.jpg -> scab
30574.4s 494 ad8770db05586b59.jpg -> complex frog_eye_leaf_spot scab
30574.4s 495 c7b03e718489f3ca.jpg -> frog_eye_leaf_spot
30574.5s 496 submission.csv saved!
30574.5s 497 
30574.5s 498 First 5 rows:
30574.5s 499 image                           labels
30574.5s 500 0  85f8cb619c66b863.jpg                             scab
30574.5s 501 1  ad8770db05586b59.jpg  complex frog_eye_leaf_spot scab
30574.5s 502 2  c7b03e718489f3ca.jpg               frog_eye_leaf_spot
30574.5s 503 
30574.5s 504 Shape: (3, 2)
30574.5s 505 Rows with empty labels: 0
30580.4s 506 /usr/local/lib/python3.12/dist-packages/mistune.py:435: SyntaxWarning: invalid escape sequence '\|'
30580.4s 507 cells[i][c] = re.sub('\\\\\|', '|', cell)
30580.6s 508 /usr/local/lib/python3.12/dist-packages/nbconvert/filters/filter_links.py:36: SyntaxWarning: invalid escape sequence '\_'
30580.6s 509 text = re.sub(r'_', '\_', text) # Escape underscores in display text
30581.3s 510 [NbConvertApp] Converting notebook __notebook__.ipynb to notebook
30581.8s 511 [NbConvertApp] Writing 2269539 bytes to __notebook__.ipynb
30584.3s 512 [NbConvertApp] Converting notebook __notebook__.ipynb to html
30585.4s 513 [NbConvertApp] Support files will be in __results___files/
30585.4s 514 [NbConvertApp] Making directory __results___files
30585.4s 515 [NbConvertApp] Making directory __results___files
30585.4s 516 [NbConvertApp] Writing 885217 bytes to __results__.html