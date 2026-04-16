11.7s 1 0.00s - Debugger warning: It seems that frozen modules are being used, which may
11.7s 2 0.00s - make the debugger miss breakpoints. Please pass -Xfrozen_modules=off
11.7s 3 0.00s - to python to disable frozen modules.
11.7s 4 0.00s - Note: Debugging will proceed. Set PYDEVD_DISABLE_FILE_VALIDATION=1 to disable this validation.
12.6s 5 0.00s - Debugger warning: It seems that frozen modules are being used, which may
12.6s 6 0.00s - make the debugger miss breakpoints. Please pass -Xfrozen_modules=off
12.6s 7 0.00s - to python to disable frozen modules.
12.6s 8 0.00s - Note: Debugging will proceed. Set PYDEVD_DISABLE_FILE_VALIDATION=1 to disable this validation.
46.7s 9 Torch: 2.10.0+cu128
46.7s 10 CUDA available: True
46.7s 11 timm: 1.0.25
46.7s 12 torchvision: 0.25.0+cu128
46.7s 13 Iterative stratification ready
46.8s 14 Train dir: /kaggle/input/competitions/plant-pathology-2021-fgvc8/train_images
46.8s 15 Test dir : /kaggle/input/competitions/plant-pathology-2021-fgvc8/test_images
46.8s 16 Device   : cuda
46.8s 17 Num GPUs : 2
46.8s 18 In notebook: True
46.8s 19 Use DDP  : False
46.8s 20 Use DataParallel: True
46.8s 21 World size: 1
46.8s 22 Num folds: 3
46.8s 23 Selected folds: [0]
46.8s 24 Train batch size (global): 32
46.8s 25 Eval image batch size: 32
46.8s 26 Image size: 518
46.8s 27 Eval mode: full_image
46.8s 28 RandAug enabled: True
46.8s 29 RandAug ops/magnitude: (2, 7)
46.8s 30 Configured workers: 2
46.8s 31 Active DataLoader workers: 0
46.8s 32 Train shape: (18632, 2)
46.8s 33 Sample submission shape: (3, 2)
46.8s 34 
46.8s 35 First 5 rows:
46.8s 36 image                           labels
46.8s 37 0  800113bb65efe69e.jpg                          healthy
46.8s 38 1  8002cb321f8bfcdf.jpg  scab frog_eye_leaf_spot complex
46.8s 39 2  80070f7fb5e2ccaa.jpg                             scab
46.8s 40 3  80077517781fb94f.jpg                             scab
46.8s 41 4  800cbf0ff87721f8.jpg                          complex
46.8s 42 
46.8s 43 Classes: ['complex', 'frog_eye_leaf_spot', 'healthy', 'powdery_mildew', 'rust', 'scab']
46.9s 44 Most common label strings:
46.9s 45 labels
46.9s 46 scab                               4826
46.9s 47 healthy                            4624
46.9s 48 frog_eye_leaf_spot                 3181
46.9s 49 rust                               1860
46.9s 50 complex                            1602
46.9s 51 powdery_mildew                     1184
46.9s 52 scab frog_eye_leaf_spot             686
46.9s 53 scab frog_eye_leaf_spot complex     200
46.9s 54 frog_eye_leaf_spot complex          165
46.9s 55 rust frog_eye_leaf_spot             120
46.9s 56 rust complex                         97
46.9s 57 powdery_mildew complex               87
46.9s 58 Name: count, dtype: int64
50.8s 59 Label matrix shape: (18632, 6)
50.8s 60 
50.8s 61 Overall per-class positive rate:
50.8s 62 scab                  0.306569
50.8s 63 healthy               0.248175
50.8s 64 frog_eye_leaf_spot    0.233577
50.8s 65 complex               0.115447
50.8s 66 rust                  0.111475
50.8s 67 powdery_mildew        0.068216
50.8s 68 dtype: float32
50.8s 69 
50.8s 70 Test images: 3
50.8s 71 
50.8s 72 Fold sizes:
50.8s 73 fold  train_size  val_size
50.8s 74 0     0       12447      6185
50.8s 75 1     1       12392      6240
50.8s 76 2     2       12425      6207
50.8s 77 
50.8s 78 Per-class validation positive rate by fold:
50.8s 79 overall_positive_rate  fold_0_val_rate  fold_1_val_rate  \
50.8s 80 complex                            0.1154           0.1159           0.1149
50.8s 81 frog_eye_leaf_spot                 0.2336           0.2346           0.2324
50.8s 82 healthy                            0.2482           0.2492           0.2470
50.8s 83 powdery_mildew                     0.0682           0.0686           0.0678
50.8s 84 rust                               0.1115           0.1119           0.1111
50.8s 85 scab                               0.3066           0.3078           0.3051
50.8s 86 
50.8s 87 fold_2_val_rate
50.8s 88 complex                      0.1155
50.8s 89 frog_eye_leaf_spot           0.2338
50.8s 90 healthy                      0.2484
50.8s 91 powdery_mildew               0.0683
50.8s 92 rust                         0.1115
50.8s 93 scab                         0.3068
51.6s 94 Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
51.6s 95 
51.6s 96 Warning: You are sending unauthenticated requests to the HF Hub. Please set a HF_TOKEN to enable higher rate limits and faster downloads.
68.8s 97 Selected timm model: vit_small_patch14_dinov2.lvd142m
68.8s 98 Normalization mean: (0.485, 0.456, 0.406)
68.8s 99 Normalization std : (0.229, 0.224, 0.225)
68.8s 100 Preview fold      : 0
68.8s 101 Train batch image count: 32
68.8s 102 First raw train image tensor shape: (3, 518, 518)
68.8s 103 First raw train image tensor dtype: torch.uint8
68.8s 104 First augmented train image tensor shape: (3, 518, 518)
68.8s 105 First augmented train image tensor dtype: torch.float32
68.8s 106 Train batch target tensor shape: (32, 6)
68.8s 107 Validation image batch tensor shape: (32, 3, 518, 518)
68.8s 108 Validation target tensor shape: (32, 6)
69.7s 109 PlantDiseaseDINOv2Model(
69.7s 110 (backbone): VisionTransformer(
69.7s 111 (patch_embed): PatchEmbed(
69.7s 112 (proj): Conv2d(3, 384, kernel_size=(14, 14), stride=(14, 14))
69.7s 113 (norm): Identity()
69.7s 114 )
69.7s 115 (pos_drop): Dropout(p=0.0, inplace=False)
69.7s 116 (patch_drop): Identity()
69.7s 117 (norm_pre): Identity()
69.7s 118 (blocks): Sequential(
69.7s 119 (0): Block(
69.7s 120 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 121 (attn): Attention(
69.7s 122 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 123 (q_norm): Identity()
69.7s 124 (k_norm): Identity()
69.7s 125 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 126 (norm): Identity()
69.7s 127 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 128 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 129 )
69.7s 130 (ls1): LayerScale()
69.7s 131 (drop_path1): Identity()
69.7s 132 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 133 (mlp): Mlp(
69.7s 134 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 135 (act): GELU(approximate='none')
69.7s 136 (drop1): Dropout(p=0.0, inplace=False)
69.7s 137 (norm): Identity()
69.7s 138 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 139 (drop2): Dropout(p=0.0, inplace=False)
69.7s 140 )
69.7s 141 (ls2): LayerScale()
69.7s 142 (drop_path2): Identity()
69.7s 143 )
69.7s 144 (1): Block(
69.7s 145 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 146 (attn): Attention(
69.7s 147 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 148 (q_norm): Identity()
69.7s 149 (k_norm): Identity()
69.7s 150 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 151 (norm): Identity()
69.7s 152 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 153 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 154 )
69.7s 155 (ls1): LayerScale()
69.7s 156 (drop_path1): Identity()
69.7s 157 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 158 (mlp): Mlp(
69.7s 159 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 160 (act): GELU(approximate='none')
69.7s 161 (drop1): Dropout(p=0.0, inplace=False)
69.7s 162 (norm): Identity()
69.7s 163 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 164 (drop2): Dropout(p=0.0, inplace=False)
69.7s 165 )
69.7s 166 (ls2): LayerScale()
69.7s 167 (drop_path2): Identity()
69.7s 168 )
69.7s 169 (2): Block(
69.7s 170 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 171 (attn): Attention(
69.7s 172 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 173 (q_norm): Identity()
69.7s 174 (k_norm): Identity()
69.7s 175 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 176 (norm): Identity()
69.7s 177 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 178 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 179 )
69.7s 180 (ls1): LayerScale()
69.7s 181 (drop_path1): Identity()
69.7s 182 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 183 (mlp): Mlp(
69.7s 184 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 185 (act): GELU(approximate='none')
69.7s 186 (drop1): Dropout(p=0.0, inplace=False)
69.7s 187 (norm): Identity()
69.7s 188 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 189 (drop2): Dropout(p=0.0, inplace=False)
69.7s 190 )
69.7s 191 (ls2): LayerScale()
69.7s 192 (drop_path2): Identity()
69.7s 193 )
69.7s 194 (3): Block(
69.7s 195 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 196 (attn): Attention(
69.7s 197 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 198 (q_norm): Identity()
69.7s 199 (k_norm): Identity()
69.7s 200 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 201 (norm): Identity()
69.7s 202 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 203 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 204 )
69.7s 205 (ls1): LayerScale()
69.7s 206 (drop_path1): Identity()
69.7s 207 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 208 (mlp): Mlp(
69.7s 209 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 210 (act): GELU(approximate='none')
69.7s 211 (drop1): Dropout(p=0.0, inplace=False)
69.7s 212 (norm): Identity()
69.7s 213 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 214 (drop2): Dropout(p=0.0, inplace=False)
69.7s 215 )
69.7s 216 (ls2): LayerScale()
69.7s 217 (drop_path2): Identity()
69.7s 218 )
69.7s 219 (4): Block(
69.7s 220 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 221 (attn): Attention(
69.7s 222 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 223 (q_norm): Identity()
69.7s 224 (k_norm): Identity()
69.7s 225 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 226 (norm): Identity()
69.7s 227 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 228 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 229 )
69.7s 230 (ls1): LayerScale()
69.7s 231 (drop_path1): Identity()
69.7s 232 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 233 (mlp): Mlp(
69.7s 234 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 235 (act): GELU(approximate='none')
69.7s 236 (drop1): Dropout(p=0.0, inplace=False)
69.7s 237 (norm): Identity()
69.7s 238 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 239 (drop2): Dropout(p=0.0, inplace=False)
69.7s 240 )
69.7s 241 (ls2): LayerScale()
69.7s 242 (drop_path2): Identity()
69.7s 243 )
69.7s 244 (5): Block(
69.7s 245 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 246 (attn): Attention(
69.7s 247 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 248 (q_norm): Identity()
69.7s 249 (k_norm): Identity()
69.7s 250 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 251 (norm): Identity()
69.7s 252 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 253 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 254 )
69.7s 255 (ls1): LayerScale()
69.7s 256 (drop_path1): Identity()
69.7s 257 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 258 (mlp): Mlp(
69.7s 259 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 260 (act): GELU(approximate='none')
69.7s 261 (drop1): Dropout(p=0.0, inplace=False)
69.7s 262 (norm): Identity()
69.7s 263 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 264 (drop2): Dropout(p=0.0, inplace=False)
69.7s 265 )
69.7s 266 (ls2): LayerScale()
69.7s 267 (drop_path2): Identity()
69.7s 268 )
69.7s 269 (6): Block(
69.7s 270 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 271 (attn): Attention(
69.7s 272 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 273 (q_norm): Identity()
69.7s 274 (k_norm): Identity()
69.7s 275 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 276 (norm): Identity()
69.7s 277 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 278 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 279 )
69.7s 280 (ls1): LayerScale()
69.7s 281 (drop_path1): Identity()
69.7s 282 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 283 (mlp): Mlp(
69.7s 284 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 285 (act): GELU(approximate='none')
69.7s 286 (drop1): Dropout(p=0.0, inplace=False)
69.7s 287 (norm): Identity()
69.7s 288 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 289 (drop2): Dropout(p=0.0, inplace=False)
69.7s 290 )
69.7s 291 (ls2): LayerScale()
69.7s 292 (drop_path2): Identity()
69.7s 293 )
69.7s 294 (7): Block(
69.7s 295 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 296 (attn): Attention(
69.7s 297 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 298 (q_norm): Identity()
69.7s 299 (k_norm): Identity()
69.7s 300 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 301 (norm): Identity()
69.7s 302 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 303 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 304 )
69.7s 305 (ls1): LayerScale()
69.7s 306 (drop_path1): Identity()
69.7s 307 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 308 (mlp): Mlp(
69.7s 309 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 310 (act): GELU(approximate='none')
69.7s 311 (drop1): Dropout(p=0.0, inplace=False)
69.7s 312 (norm): Identity()
69.7s 313 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 314 (drop2): Dropout(p=0.0, inplace=False)
69.7s 315 )
69.7s 316 (ls2): LayerScale()
69.7s 317 (drop_path2): Identity()
69.7s 318 )
69.7s 319 (8): Block(
69.7s 320 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 321 (attn): Attention(
69.7s 322 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 323 (q_norm): Identity()
69.7s 324 (k_norm): Identity()
69.7s 325 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 326 (norm): Identity()
69.7s 327 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 328 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 329 )
69.7s 330 (ls1): LayerScale()
69.7s 331 (drop_path1): Identity()
69.7s 332 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 333 (mlp): Mlp(
69.7s 334 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 335 (act): GELU(approximate='none')
69.7s 336 (drop1): Dropout(p=0.0, inplace=False)
69.7s 337 (norm): Identity()
69.7s 338 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 339 (drop2): Dropout(p=0.0, inplace=False)
69.7s 340 )
69.7s 341 (ls2): LayerScale()
69.7s 342 (drop_path2): Identity()
69.7s 343 )
69.7s 344 (9): Block(
69.7s 345 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 346 (attn): Attention(
69.7s 347 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 348 (q_norm): Identity()
69.7s 349 (k_norm): Identity()
69.7s 350 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 351 (norm): Identity()
69.7s 352 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 353 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 354 )
69.7s 355 (ls1): LayerScale()
69.7s 356 (drop_path1): Identity()
69.7s 357 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 358 (mlp): Mlp(
69.7s 359 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 360 (act): GELU(approximate='none')
69.7s 361 (drop1): Dropout(p=0.0, inplace=False)
69.7s 362 (norm): Identity()
69.7s 363 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 364 (drop2): Dropout(p=0.0, inplace=False)
69.7s 365 )
69.7s 366 (ls2): LayerScale()
69.7s 367 (drop_path2): Identity()
69.7s 368 )
69.7s 369 (10): Block(
69.7s 370 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 371 (attn): Attention(
69.7s 372 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 373 (q_norm): Identity()
69.7s 374 (k_norm): Identity()
69.7s 375 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 376 (norm): Identity()
69.7s 377 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 378 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 379 )
69.7s 380 (ls1): LayerScale()
69.7s 381 (drop_path1): Identity()
69.7s 382 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 383 (mlp): Mlp(
69.7s 384 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 385 (act): GELU(approximate='none')
69.7s 386 (drop1): Dropout(p=0.0, inplace=False)
69.7s 387 (norm): Identity()
69.7s 388 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 389 (drop2): Dropout(p=0.0, inplace=False)
69.7s 390 )
69.7s 391 (ls2): LayerScale()
69.7s 392 (drop_path2): Identity()
69.7s 393 )
69.7s 394 (11): Block(
69.7s 395 (norm1): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 396 (attn): Attention(
69.7s 397 (qkv): Linear(in_features=384, out_features=1152, bias=True)
69.7s 398 (q_norm): Identity()
69.7s 399 (k_norm): Identity()
69.7s 400 (attn_drop): Dropout(p=0.0, inplace=False)
69.7s 401 (norm): Identity()
69.7s 402 (proj): Linear(in_features=384, out_features=384, bias=True)
69.7s 403 (proj_drop): Dropout(p=0.0, inplace=False)
69.7s 404 )
69.7s 405 (ls1): LayerScale()
69.7s 406 (drop_path1): Identity()
69.7s 407 (norm2): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 408 (mlp): Mlp(
69.7s 409 (fc1): Linear(in_features=384, out_features=1536, bias=True)
69.7s 410 (act): GELU(approximate='none')
69.7s 411 (drop1): Dropout(p=0.0, inplace=False)
69.7s 412 (norm): Identity()
69.7s 413 (fc2): Linear(in_features=1536, out_features=384, bias=True)
69.7s 414 (drop2): Dropout(p=0.0, inplace=False)
69.7s 415 )
69.7s 416 (ls2): LayerScale()
69.7s 417 (drop_path2): Identity()
69.7s 418 )
69.7s 419 )
69.7s 420 (norm): LayerNorm((384,), eps=1e-06, elementwise_affine=True)
69.7s 421 (fc_norm): Identity()
69.7s 422 (head_drop): Dropout(p=0.0, inplace=False)
69.7s 423 (head): Identity()
69.7s 424 )
69.7s 425 (head): Sequential(
69.7s 426 (0): LayerNorm((384,), eps=1e-05, elementwise_affine=True)
69.7s 427 (1): Dropout(p=0.3, inplace=False)
69.7s 428 (2): Linear(in_features=384, out_features=256, bias=True)
69.7s 429 (3): GELU(approximate='none')
69.7s 430 (4): Dropout(p=0.2, inplace=False)
69.7s 431 (5): Linear(in_features=256, out_features=6, bias=True)
69.7s 432 )
69.7s 433 )
69.7s 434 
69.7s 435 Trainable parameters after freezing backbone: 100870
70.4s 436 
70.4s 437 ============ Running Selected Fold 0 ============
70.4s 438 Checkpoint path: /kaggle/working/best_dinov2_small_plant_pathology_fold0.pth
70.4s 439 Distributed training: False
70.4s 440 DataParallel training: True
70.4s 441 Global train batch size: 32
70.4s 442 Eval image batch size: 32
70.4s 443 Trainable parameters after freezing backbone: 100870
3296.4s 444 Head training | Epoch 01/3 | train_loss=0.2585 | train_f1=0.6551 | val_image_f1=0.7699 | val_mode=full_image
6221.5s 445 Head training | Epoch 02/3 | train_loss=0.2078 | train_f1=0.7365 | val_image_f1=0.8089 | val_mode=full_image
9157.7s 446 Head training | Epoch 03/3 | train_loss=0.1934 | train_f1=0.7524 | val_image_f1=0.8156 | val_mode=full_image
9157.8s 447 Reloaded best checkpoint from stage: Head training (val_f1=0.8156, mode=full_image)
9157.8s 448 Trainable parameters after partial unfreeze: 3652102
9157.8s 449 Backbone parameter groups: 30
9157.8s 450 Head parameter groups    : 6
12104.1s 451 Fine-tuning | Epoch 01/3 | train_loss=0.1367 | train_f1=0.8327 | val_image_f1=0.8765 | val_mode=full_image
15026.5s 452 Fine-tuning | Epoch 02/3 | train_loss=0.1081 | train_f1=0.8658 | val_image_f1=0.8862 | val_mode=full_image
17985.7s 453 Fine-tuning | Epoch 03/3 | train_loss=0.0968 | train_f1=0.8788 | val_image_f1=0.8959 | val_mode=full_image
17985.8s 454 Reloaded best checkpoint from stage: Fine-tuning (val_f1=0.8959, mode=full_image)
18991.7s 455 Selected fold run finished.
18991.7s 456 
18991.7s 457 Per-selected-fold summary:
18991.7s 458 fold  train_size  val_size   best_stage  best_epoch  best_val_f1  \
18991.7s 459 0     0       12447      6185  Fine-tuning           3     0.895925
18991.7s 460 
18991.7s 461 checkpoint_path
18991.7s 462 0  /kaggle/working/best_dinov2_small_plant_pathol...
18991.7s 463 
18991.7s 464 Validation summary across selected folds:
18991.7s 465 validation_mode  mean_val_f1  std_val_f1
18991.7s 466 0      full_image       0.8959         0.0
18991.7s 467 
18991.7s 468 Validation mode: full_image
18991.8s 469 Validation summary across selected folds:
18991.9s 470 validation_mode  mean_val_f1  std_val_f1
18991.9s 471 0      full_image       0.8959         0.0
18991.9s 472 
18991.9s 473 Validation mode: full_image
18991.9s 474 Mean F1: 0.8959 +/- 0.0000
18991.9s 475 Ensemble folds: [0]
18993.2s 476 Ensemble folds: [0]
18993.2s 477 Checkpoint stages: {0: 'Fine-tuning'}
18993.2s 478 Evaluation mode: full_image
18993.2s 479 
18993.2s 480 Sample predictions:
18993.2s 481 85f8cb619c66b863.jpg -> scab
18993.2s 482 ad8770db05586b59.jpg -> complex frog_eye_leaf_spot scab
18993.2s 483 c7b03e718489f3ca.jpg -> frog_eye_leaf_spot
18993.3s 484 submission.csv saved!
18993.3s 485 
18993.3s 486 First 5 rows:
18993.3s 487 image                           labels
18993.3s 488 0  85f8cb619c66b863.jpg                             scab
18993.3s 489 1  ad8770db05586b59.jpg  complex frog_eye_leaf_spot scab
18993.3s 490 2  c7b03e718489f3ca.jpg               frog_eye_leaf_spot
18993.3s 491 
18993.3s 492 Shape: (3, 2)
18993.3s 493 Rows with empty labels: 0
18999.6s 494 /usr/local/lib/python3.12/dist-packages/mistune.py:435: SyntaxWarning: invalid escape sequence '\|'
18999.6s 495 cells[i][c] = re.sub('\\\\\|', '|', cell)
18999.9s 496 /usr/local/lib/python3.12/dist-packages/nbconvert/filters/filter_links.py:36: SyntaxWarning: invalid escape sequence '\_'
18999.9s 497 text = re.sub(r'_', '\_', text) # Escape underscores in display text
19000.8s 498 [NbConvertApp] Converting notebook __notebook__.ipynb to notebook
19001.2s 499 [NbConvertApp] Writing 1880449 bytes to __notebook__.ipynb
19003.9s 500 [NbConvertApp] Converting notebook __notebook__.ipynb to html
19005.1s 501 [NbConvertApp] Support files will be in __results___files/
19005.1s 502 [NbConvertApp] Making directory __results___files
19005.1s 503 [NbConvertApp] Making directory __results___files
19005.1s 504 [NbConvertApp] Writing 640006 bytes to __results__.html