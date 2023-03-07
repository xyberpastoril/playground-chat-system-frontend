<script>
    import { onMount } from 'svelte';
    import { Form, FormGroup, Label, Input, Button, Container, Row } from 'sveltestrap';
    
    let username = '';
    let password = '';
    
    function handleSubmit(event) {
        event.preventDefault();
        const formData = new FormData(event.target);
        const email = formData.get('email');
        const password = formData.get('password');
        console.log(`Email: ${email}, Password: ${password}`);
        // perform any additional logic or API calls here
    }
    
    onMount(() => {
        // initialize any Sveltestrap components here
        Form.init();
        FormGroup.init();
        Label.init();
        Input.init();
        Button.init();
    });
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<Container class="d-flex align-items-center justify-content-center" style="height: 100vh;">
    <Row>
        <h1>Login</h1>
        <Form on:submit={handleSubmit}>
            <FormGroup floating label="Email">
                <Input type="email" name="email"></Input>
            </FormGroup>
            <FormGroup floating label="Password">
                <Input type="password" name="password"></Input>
            </FormGroup>
            <Button type="submit" color="primary">Login</Button>
        </Form>
    </Row>
</Container>