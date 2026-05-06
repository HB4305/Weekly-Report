# AI Usage Declaration — Yum Recipe

**Group 03** | Project: Yum Recipe

---

## Nguyễn Duy Thịnh (23127122)

**Create post & Like / Share post / Comment on post**
Claude Sonnet 4.6 + Claude Opus 4.6 (Anthropic), claude.ai; Gemini Thinking 3 (Google), accessed April 11, 2026; prompt: *"build social feature group scaffolding — post, like, share, comment repository"*; AI generated social related services and repositories; later adjusts and wires up some endpoints to match existing team codebase.

**View personalized feed**
Stitch (Gemini 3.1 Pro) + Claude Sonnet 4.6 (Anthropic), claude.ai, accessed March 8–12 & March 26, 2026; prompts: MVVM feed brainstorm; *"api design for infinite scroll social feed"*; *"rewrite item_feed_post.xml with 4 post-type states using ViewStubs"*; AI generated `fragment_feed.xml`, `item_feed_post.xml`, 4 post-type XML includes; student independently implemented backend social endpoints.

**Create and view blog posts / Share images and experiences alongside recipes**
Claude Sonnet 4.6 (Anthropic), claude.ai, accessed April 3, 2026; AI generated `PostMapper.java`, `fragment_post_detail.xml`, `item_comment.xml`; student refactored DTOs for consistency between Android client and server.

**Create challenges (Admin)**
Claude Sonnet 4.6 (Anthropic), accessed May 5, 2026; prompt: *"Add create challenge view to match existing endpoints"*; AI generated `CreateChallengeFragment.java`, `ChallengeViewModel.java`; later tested manually on Android and verified API integration.

**Vote in challenges / Award profile titles**


**Share blog posts**
Claude Sonnet 4.6 (Anthropic), accessed April 11, 2026; prompt: *"Create sharing functionality for blog posts, replicate the sharing post functionality but without adding photos"*; AI modified `menu_article_viewer.xml`, added `ArticleShareBottomSheet.java`, modified `ArticleViewerFragment.java`, modified `fragment_article_viewer.xml` to add share button; student tested on Android and verified sharing flow.

**Export recipe to PDF / Export recipe to image with QR code**


---

## Lâm Hữu Khánh (23127205)

**Sign up / Sign in / Forgot password / Email notifications**
Gemini 3 Pro (Google), gemini.google.com, accessed 17:00, March 14, 2026; prompts: *"Implement Spring Boot APIs for User Registration and Secure Login using JWT"* / *"Create an Email Service to handle Forgot Password and Password Reset"*; AI generated `AuthController.java`, `AuthService.java`, JWT security config, Email Service, and password reset token handling; student integrated JWT with custom `UserDetails`, verified password encryption and token expiry, tested end-to-end auth flow on Android.

**Sign in UI / Login binding / Change password (UI layer)**
Claude Opus (Anthropic), accessed March 18, 2026; prompt: *"Complete the UI screens (Login/Signup/ForgotPassword), bind API to UI, check security for APIs"*; AI generated auth fragments (`fragment_login.xml`, `fragment_register.xml`, `fragment_forgot_password.xml`, `fragment_reset_password.xml`), `AuthViewModel.java`, `AuthRepository.java`, `JwtService.java`, `JwtAuthFilter.java`; student added custom OTP styling, Google OAuth verification, and JWT with `EncryptedSharedPreferences` (AES256-GCM).

**Edit personal profile (Avatar, bio, specialty)**
Claude Opus 4.6 (Anthropic) via Claude Code CLI, accessed March 29–April 4, 2026; prompts: implement Own Profile, Other Profile, and Edit Profile UIs from Figma; AI generated `fragment_profile.xml`, `fragment_edit_profile.xml`, `ProfileFragment.java`, `EditProfileFragment.java`, `ProfileViewModel.java`, `ProfileRepository.java`, and backend `ProfileController.java`; student wrote camera/gallery launcher via Activity Result API, `BottomSheetDialog`, dual-mode `isOwnProfile` logic, Glide bitmap-to-base64 encoding, `ViewPager2` tab mediator, and dark-theme XML customizations.

**Account privacy settings / Manage connections (Followers/Following)**
Claude Opus 4.6 (Anthropic), accessed April 6–11, 2026; prompt: *"add private profile with mutual-follow access check; migrate image storage from Base64 to Cloudinary"*; AI suggested implementation flow and code-level changes for mutual-follow privacy and Cloudinary refactor; student adjusted to existing Spring Boot and Android structure, verified API integration, error handling, and navigation behavior.

**Push notifications / App preferences / Manage users (Ban/Unban) / Moderate complaints**
No AI usage declared.

---

## Lê Mai Hoài Bảo (23127326)

**Search recipe / Search post / Search user**
Claude Opus 4.6 (Anthropic), accessed 14:30, April 8, 2026; prompt: *"add a search bar to dashboard — pop-up with title input, difficulty filter, ingredient selector; show search results page"*; AI generated search bar UI, pop-up search interface, search results page, and API integration logic; student tested and verified against project requirements.

**Create recipe**
Gemini 3.1 Pro (Google) + Claude Opus 4.6 (Anthropic), accessed March 18 & April 2, 2026; prompts: *"Implement the API to create a new recipe and create the unit test"* / create recipe UI with FAB → nav → form with backend integration; AI generated `RecipeController.java` (create endpoint), `RecipeServiceTest.java`, `CreateRecipeFragment.java`, `CreateRecipeViewModel.java`, all related DTOs and drawables; student ran end-to-end tests, verified DB, reviewed naming and logic.

**View recipe**
Claude Opus (Anthropic), accessed 17:00, March 28, 2026; prompt: *"Implement a UI to view recipe details via GET api/recipes/{id}"*; AI generated `RecipeDetailFragment.java`, `IngredientAdapter.java`, `InstructionAdapter.java`, all related DTOs and drawables; student ran app via hardcoded recipe ID, verified UI against design mockup, and tested interactions.

**Update recipe**
Claude Opus (Anthropic), accessed 13:00, March 21, 2026; prompt: *"Implement the API to edit an existing recipe"*; AI generated edit endpoint in `RecipeController.java`, `RecipeService.java`, `UpdateRecipeRequest.java`; student tested full/partial update, non-existent ID, and unauthorized-owner cases via Swagger UI.

**Delete recipe**
Claude Opus (Anthropic), accessed 16:00, March 21, 2026; prompt: *"Implement the API to delete a recipe"*; AI generated delete endpoint with ownership validation in `RecipeController.java` and `RecipeService.java`; student tested valid/invalid/unauthorized scenarios via Swagger UI.

**Cooking timer**
Claude Opus (Anthropic), accessed 15:00, March 28, 2026; prompt: *"Implement timer functionality for cooking steps"*; AI generated `StepTimerResponse.java`, DB migration, `GET /api/recipes/{id}/steps/{step}/timer` endpoint; student verified backward-compatible migration and tested duration formatting (e.g. 480 → "8 min", 150 → "2 min 30 sec") via Postman.

**Hands-free mode**
Claude Opus (Anthropic), accessed 16:00, March 28, 2026; prompt: *"Implement hands-free cooking mode using SpeechRecognizer API in Backend"*; AI generated `VoiceCommandType.java` (11 intents), `CookingModeService.java`, `CookingModeController.java` (`POST /api/cooking-mode/command`); student tested intent parsing and TTS responses via Swagger UI.

**Save recipe as draft / Manage gallery / Manage favorite recipes**
No AI usage declared.

---

## Lê Anh Duy (23127357)

**Track fridge inventory / Suggest recipes based on ingredients**
Stitch (Gemini 3.1 Pro) + ChatGPT 5.1 (OpenAI) + Claude Sonnet 4.6 (Anthropic), accessed March 8–13, 2026; prompts: generate UI for fridge and ingredient management views; AI generated `fragment_fridge_manager.xml`, `fragment_add_fridge_item.xml`, `component_item_fridge_category.xml`, `component_item_ingredient_card.xml`, `component_suggestion_list_item.xml`.

**Generate daily meal plans / Estimate calorie counts**
Gemini 3.1 Pro + ChatGPT 5.1 (OpenAI) + Claude Sonnet 4.6 (Anthropic), accessed March 14–28, 2026; prompts: generate meal planner UI, user stat setup UI, and mock data; AI generated `fragment_meal_planner.xml`, `fragment_user_stat_setup.xml`, `UserStatSetupViewModel.java`, Meal Plan mock data; student integrated into the app.

**Visualize trending recipes / Visualize user ingredient preferences**
Claude Sonnet 4.6 (Anthropic) + Codex 5.3 (OpenAI), accessed April 9–11, 2026; prompts: admin dashboard UI with ingredient and recipe trend charts; AI generated DB changelogs (`create-recipe-metrics`, `create-ingredient-trend`, `create-user-activity-log`, `create-daily-trend-snapshot`), `ActivityLoggerPersistence.java`, admin chart UI; student integrated with backend API and tested charts.

**AI-powered recipe recommendations / Suggest ingredient substitutions / Generate grocery lists / Link grocery list items**
No AI usage declared.
