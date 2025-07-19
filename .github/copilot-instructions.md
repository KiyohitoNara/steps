# Test Naming Guidelines
Conventions for tests using **XCTest** and **swift-testing**.

## General
- Follow **Given–When–Then**.
- Be descriptive, concise, present tense.
- No punctuation.

## XCTest
- Function name: **camelCase**, starts with `test`, expresses Given–When–Then.
- Example:
```swift
func testGivenUserIsLoggedInWhenFetchingProfileThenReturnsProfileData() {
    // Arrange, Act, Assert
}
```

## swift-testing
- Use @test("…") for description (all lowercase, Given–When–Then).
- Function name: short and meaningful.
- Example:
```swift
@test("given user is logged in when fetching profile then returns profile data")
func profileFetching() async throws {
    // Arrange, Act, Assert
}
```
