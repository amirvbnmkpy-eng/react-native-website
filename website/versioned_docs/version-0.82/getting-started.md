---
import React, { useState } from 'react';
import { View, TextInput, Button, StyleSheet, Alert } from 'react-native';

export default function LoginScreen({ navigation }) {
  const [phone, setPhone] = useState('');

  const handleLogin = () => {
    if (phone.length >= 10) {
      navigation.navigate('Home');
    } else {
      Alert.alert('خطا', 'شماره معتبر وارد کنید');
    }
  };

  return (
    <View style={styles.container}>
      <TextInput
        placeholder="شماره تلفن خود را وارد کنید"
        keyboardType="phone-pad"
        value={phone}
        onChangeText={setPhone}
        style={styles.input}
      />
      <Button title="ورود" onPress={handleLogin} />
    </View>
  );
}

const styles = StyleSheet.create({
  container: { flex: 1, justifyContent: 'center', padding: 20 },
  input: { borderWidth: 1, padding: 10, marginBottom: 20 },
});
import React from 'react';
import React from 'react';
import { View, Text, Button, StyleSheet } from 'react-native';

export default function ProjectScreen({ route }) {
  const { name } = route.params;

  return (
    <View style={styles.container}>
      <Text style={styles.title}>{name}</Text>
      <Button title="ساخت فایل و پیش‌نمایش" onPress={() => {}} />
      <Button title="تبلیغات (پولی)" onPress={() => {}} />
      <Button title="پرداخت بازار و مایکت" onPress={() => {}} />
      <Button title="مشخصات برنامه" onPress={() => {}} />
      <Button title="فایل دلخواه" onPress={() => {}} />
    </View>
  );
}

const styles = StyleSheet.create({
  container: { flex: 1, padding: 20 },
  title: { fontSize: 22, marginBottom: 20 },
});

import { NavigationContainer } from '@react-navigation/native';
import { createNativeStackNavigator } from '@react-navigation/native-stack';
import LoginScreen from './screens/LoginScreen';
import HomeScreen from './screens/HomeScreen';
import ProjectScreen from './screens/ProjectScreen';

const Stack = createNativeStackNavigator();

export default function App() {
  return (
    <NavigationContainer>
      <Stack.Navigator initialRouteName="Login">
        <Stack.Screen name="Login" component={LoginScreen} />
        <Stack.Screen name="Home" component={HomeScreen} />
        <Stack.Screen name="Project"
component={ProjectScreen} />
      </Stack.Navigator>
    </NavigationContainer>
  );
import React from 'react';
import { View, Text, Button, FlatList } from 'react-native';

export default function HomeScreen({ navigation }) {
  const projects = Array.from({ length: 20 }, (_, i) => `پروژه ${i + 1}`);

  return (
    <View style={{ flex: 1, padding: 20 }}>
      <Text style={{ fontSize: 18, marginBottom: 10 }}>پروژه‌های شما:</Text>
      <FlatList
        data={projects}
        keyExtractor={(item) => item}
        renderItem={({ item }) => (
          <Button title={item} onPress={() => navigation.navigate('Project', { name: item })} />
        )}
      />
    </View>
  );
}} 
