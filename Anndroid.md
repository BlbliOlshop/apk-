@Test
public void greeterSaysHello() {
    onView(withId(R.id.name_field)).perform(typeText("BliOlshop"));
    onView(withId(R.id.greet_button)).perform(click());
    onView(withText("Hello Steve!")).check(matches(isDisplayed()));
}
